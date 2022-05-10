class Counter:
    def __init__(self, min_value=0, max_value=100, get=None):
        self.min_value = min_value
        self.max_value = max_value
        self.get = get
    def increase(self):
        if self.get < self.max_value and self.get >= self.min_value:           
            self.get += 1
        elif self.get == None:
            self.get = 1
        else:
            pass


    def get_current_value(self):
        return self.get


x = Counter(min_value=1, max_value=100, get=3)

print(x.increase())
print(x.get_current_value())
