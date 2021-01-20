

def df_dx(x, y):

    return round((36*(x**5) + 8*y*y*(x**3) + 20*x + 6*y - 6), 40)

def df_dy(x,y):

    return (4*y*(x**4) + 20*y + 6*x)

def modul(x, y):

    return (x*x + y*y)**0.5

def f(x,y):
    return (6*x**6 + 2*x**4 * y**2 + 10*x**2 + 10*y**2 +6*x*y - 6*x + 4)
	

x = 0
y = 0
eps = 1e-5
new_x = -0.01
new_y = -0.01
l = -0.000001

i = 0
while modul(new_x - x, new_y - y) > eps and i < 10e5:
    t_1 = new_x
    t_2 = new_y
    new_x = x + l*df_dx(x, y)
    new_y = y + l*df_dy(x,y)
    #print(df_dx(x, y), df_dy(x,y))
    x = t_1
    y = t_2
    i += 1
#print("-----------------")
#print(new_x, new_y)
print(f(new_x, new_y))
