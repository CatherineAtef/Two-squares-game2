print("Welcome to ~Two Square Game~")
B = [[1,2,3,4],[5,6,7,8],[9,10,11,12],[13,14,15,16]]
c = []
print(B[0][0],"",B[0][1],"",B[0][2],"",B[0][3])
print(B[1][0],"",B[1][1],"",B[1][2],"",B[1][3])
print(B[2][0],"",B[2][1],B[2][2],B[2][3])
print(B[3][0],B[3][1],B[3][2],B[3][3])

check = 0

for i in range(4):
    
    K = int(input("First player,Please enter your first number: "))
    L = int(input("First player,Please enter your second number: "))
    
    if K in c or L in c:
        print("Opps you can't enter the same number twice")
    else :
        c.append(K)
        c.append(L)
        for z in range(4):
            for o in range(4):
                if B[z][o] == K:
                    B[z][o] = "X"
                if B[z][o] == L:
                    B[z][o] = "X"
        print(B[0][0],"",B[0][1],"",B[0][2],"",B[0][3])
        print(B[1][0],"",B[1][1],"",B[1][2],"",B[1][3])
        print(B[2][0],"",B[2][1],B[2][2],B[2][3])
        print(B[3][0],B[3][1],B[3][2],B[3][3])


        if (B[0][0] != "X" and B[0][1] != "X") or (B[0][1] != "X" and B[0][2] != "X") or (B[0][2] != "X" and B[0][3] != "X") or (B[1][0] != "X" and B[1][1] != "X") or (B[1][1] != "X" and B[1][2] != "X") or (B[1][2] != "X" and B[1][3] != "X") or (B[2][0] != "X" and B[2][1] != "X") or  (B[2][1] != "X" and B[2][2] != "X") or  (B[2][2] != "X" and B[2][3] != "X") or  (B[3][0] != "X" and B[3][1] != "X") or (B[3][1] != "X" and B[3][2] != "X") or (B[3][2] != "X" and B[3][3] != "X") or (B[0][0] != "X" and B[1][0] != "X") or (B[1][0] != "X" and B[2][0] != "X") or (B[2][0] != "X" and B[3][0] != "X") or (B[0][1] != "X" and B[1][1] != "X") or (B[1][1] != "X" and B[2][1] != "X") or (B[2][1] != "X" and B[3][1] != "X") or (B[0][2] != "X" and B[1][2] != "X") or (B[1][2] != "X" and B[2][2] != "X") or (B[2][2] != "X" and B[3][2] != "X") or (B[0][3] != "X" and B[1][3] != "X") or (B[1][3] != "X" and B[2][3] != "X") or (B[2][3] != "X" and B[3][3] != "X"):
            ex=1
        else:
            print("First player won")
            break

    K = int(input("Second player,Please enter your first number: "))
    L = int(input("Second player,Please enter your second number: "))
   
    if K in c or L in c:
        print("Opps you can't enter the same number twice")
    else :
        c.append(K)
        c.append(L)
        for z in range(4):
            for o in range(4):
                if B[z][o] == K:
                    B[z][o] = "X"
                if B[z][o] == L:
                    B[z][o] = "X"
        print(B[0][0],"",B[0][1],"",B[0][2],"",B[0][3])
        print(B[1][0],"",B[1][1],"",B[1][2],"",B[1][3])
        print(B[2][0],"",B[2][1],B[2][2],B[2][3])
        print(B[3][0],B[3][1],B[3][2],B[3][3])


        if (B[0][0] != "X" and B[0][1] != "X") or (B[0][1] != "X" and B[0][2] != "X") or (B[0][2] != "X" and B[0][3] != "X") or (B[1][0] != "X" and B[1][1] != "X") or (B[1][1] != "X" and B[1][2] != "X") or (B[1][2] != "X" and B[1][3] != "X") or (B[2][0] != "X" and B[2][1] != "X") or  (B[2][1] != "X" and B[2][2] != "X") or  (B[2][2] != "X" and B[2][3] != "X") or  (B[3][0] != "X" and B[3][1] != "X") or (B[3][1] != "X" and B[3][2] != "X") or (B[3][2] != "X" and B[3][3] != "X") or (B[0][0] != "X" and B[1][0] != "X") or (B[1][0] != "X" and B[2][0] != "X") or (B[2][0] != "X" and B[3][0] != "X") or (B[0][1] != "X" and B[1][1] != "X") or (B[1][1] != "X" and B[2][1] != "X") or (B[2][1] != "X" and B[3][1] != "X") or (B[0][2] != "X" and B[1][2] != "X") or (B[1][2] != "X" and B[2][2] != "X") or (B[2][2] != "X" and B[3][2] != "X") or (B[0][3] != "X" and B[1][3] != "X") or (B[1][3] != "X" and B[2][3] != "X") or (B[2][3] != "X" and B[3][3] != "X"):
            ex=1
        elif check <= 2:
            print("Second player won")
            break

    check = check + 1 
if check ==4:
    print("No winner")


