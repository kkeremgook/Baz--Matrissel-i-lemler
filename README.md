# Matrisi çıktıya gönderme
import random

# a = [[1,2,3,4],
#      [5,6,7,8,],
#      [9,10,11,12],
#      [13,14,15,16]]
# for i in range(len(a)):
#     for j in range(len(a[i])):
#         print(a[i][j], end = " ")
#     print()


# M x N boyutlu sıfır matrisi yapma
#
# m = 6
# n =4
# a = [[0 for i in range(m)] for i in range(n)]
# print(a)


# iki matrisin toplanması
#
# import random
# def MatrisiEkranaYaz(Matris,Ad):
#     print(Ad)
#     for i in range(len(Matris)):
#         for j in range(len(Matris)):
#             print(([i][j], end=" "))
#         print()
#
# A = [[int(10*random.random()) for i in range(4)] for j in range(4)]
# MatrisiEkranaYaz(A,A)
#
# B =  [[int(10*random.random()) for i in range(4)] for j in range(4)]
# MatrisiEkranaYaz(B,B)
#
# C = [[0 for i in range(4)] for j in range(4)]
# for i in range(4):
#     for j in range(4):
#         C[i][j] = A[i][j] + B[i][j]
# MatrisiEkranaYaz(C,'C')



# import random
# def MatrisYaz(Matris,Ad):
#     print(Ad)
#     for i in range(len(Matris)):
#         for j in range(len(Matris[i])):
#             print(Matris[i][j], end=" ")
#         print()
#     print()
#
# m = 2;
# n = 3
# Matris1 = [[round(random.random() * 10) for i in range(n)] for j in range(m)]
# Matris2 = [[round(random.random() * 10) for i in range(n)] for j in range(m)]
# Matris3 = [[0 for i in range(n)] for j in range(m)]
#
# for i in range(len(Matris3)):
#     for j in range(len(Matris3[i])):
#         Matris3[i][j] = Matris1[i][j] + Matris2[i][j]
# MatrisYaz(Matris1, Matris1)
# MatrisYaz(Matris2, Matris2)
# MatrisYaz(Matris3, Matris3)



# MATRİSİN SATIR VE SÜTUN TOPLAMINI HESAPLAYAN PROGRAM

# import random
# def MatrisiYaaz(Matris, Ad):
#     print(Ad)
#     for i in range(len(Matris)):
#         for j in range(len(Matris[i])):
#             print(Matris[i][j], end= " ")
#         print()
#
# b = 2 ; A = [[int(10*random.random())for i in range(b)]for j in range(b)]
# MatrisiYaaz(A,'A')
#
# satirtop = []
# for j in range(b):
#     top = 0
#     for i in range(b):
#         top += A[i][j]
#     satirtop.append(top)
# print("Satirtop",satirtop)


# MATRİSTEKİ EN BÜYÜK SAYIYI BUL

import random

satir_sayisi = int(input("matris satırı girin: "))
sutun_sayisi = int(input("matrise sütun girin: "))

matris = [[int(random.random()*10)for i in range(satir_sayisi)]for j in range(sutun_sayisi)]

print("oluşturulan matris: ")
for satir in matris:
    print(satir)

en_buyuk_sayi = max(max(satir) for satir in matris)

print(f"en büyük sayi: {en_buyuk_sayi}")
