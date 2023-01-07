from basepokemon import BasePokemon, BaseMove, Type

class Pokemon(BasePokemon):
    def __init__(self):
        BasePokemon.__init__(self)
        # Has to sum to 100
        self.spend_hp(10)
        self.spend_attack(10)
        self.spend_defence(80)
        self.add_move(Shes_truck())
        self.add_move(Machetazo())
        self.add_move(Improvises())
        self.add_move(April_Kiss())
        self.set_type(Type.FIRE)
        self.move = 0
        self.moves = ["Shes_truck", "Machetazo", "Improvises", "April_Kiss"]


    def get_name(self):
        return "Machetender"

    def choose_move(self, enemy):
        mov = self.moves[self.move]
        self.move = self.move + 1 if self.move < len(self.moves) - 1 else 0
        return self.get_move_by_name(mov)

class Shes_truck(BaseMove):
    def __init__(self):
        BaseMove.__init__(self)
        self.choose_uses(1)
        self.set_type(Type.FIRE)

    def get_name(self):
        return "Shes_truck"

class Machetazo(BaseMove):
    def __init__(self):
        BaseMove.__init__(self)
        self.choose_uses(1)
        self.set_type(Type.EARTH)

    def get_name(self):
        return "Machetazo"


class Improvises(BaseMove):
    def __init__(self):
        BaseMove.__init__(self)
        self.choose_uses(1)
        self.set_type(Type.NORMAL)

    def get_name(self):
        return "Improvises"


class April_Kiss(BaseMove):
    def __init__(self):
        BaseMove.__init__(self)
        self.choose_uses(1)
        self.set_type(Type.WATER)

    def get_name(self):
        return "April_Kiss"
