I worked about battery section over the path. Algorithms are  used for path finding. Then the battery is decreage by loop over path array.

If it falls below 10%, the battery will be recharged.

There is no difference between UCS and Ester Search in my code. Because I figured out path  first and then worked on it. 
But generally among them A* serch is very efficient in search. Through the heuristic function, it knows in advance how far the destination is. 
But in case of UCS search it has to do backtracking.

the funtion is:


# Battery Charging point and management
    def battery_manager(self, path):
        self.recharge()
        charging_point = []
        charge=[]

        for i in range(len(path)):
            if self.current_charge() <= 10:
                charging_point.append(path[i])
                self.recharge()  
                charge.append(self.charge_level)
            elif path[i] != (0, 0):
                self.charge_level = self.current_charge() - 10
                charge.append(self.charge_level)
                
        return charging_point ,charge
