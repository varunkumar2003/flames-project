# flames-project
def flames(X,Y):
    if((len(X)+len(Y))%2==0 and (len(X)+len(Y))%3==0):
        print("you both are in love but will not marry")
    elif((len(X)+len(Y))%3==0 and (len(X)+len(Y))%2!=0):
        print("you both are best friends")
    elif((len(X)+len(Y))%3!=0 and (len(X)+len(Y))%2==0):
        print("you both are brothers and sisters")
    elif((len(X)+len(Y))%3!=0 and (len(X)+len(Y))%2!=0):
        print("you both will marry")
    else: print("you both are strangers")
    
    

S=input()
T=input()
X=list(S)
Y=list(T)
for elem1 in list(X):
    for elem2 in list(Y):
        if(elem1==elem2):
            X.remove(elem1)
            Y.remove(elem2)
flames(X,Y)
