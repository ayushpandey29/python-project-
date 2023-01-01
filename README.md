# python-project-
n = int(input("Enter number of pieces to cut the cake : "))



def checkNequalpieces(num:int):

    if 360%num == 0 :
        return True
    else:
        return False

def checkNpieces(num:int):
    maxnumofpieces = 360
    if num<=360:
        return True
    else:
        return False

def CheckNoTwoEqualPieces(num:int):
    sumofangles = (num*(num-1))/2

    if sumofangles <= 360:
        return True
    else:
        return False


if checkNequalpieces(n):
    print(f'1. Yes, It is possible to cut a cake into {n} Equal pieces')
elif checkNequalpieces(n) == False:
    print(f'1. No, It is not possible to cut a cake into {n} Equal pieces')

if checkNpieces(n):
    print(f'2. Yes, It is possible to cut a cake into {n} pieces')
elif checkNpieces(n) == False:
    print(f'2. No, It is not possible to cut a cake into {n} pieces')

if CheckNoTwoEqualPieces(n):
    print(f'3. Yes, It is possible to cut a cake into {n} pieces such that no two pieces are equal')
elif CheckNoTwoEqualPieces(n) == False:
    print(f'3. No, It is not possible to cut a cake into {n} pieces such that no two pieces are equal')
