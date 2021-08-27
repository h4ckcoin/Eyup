Number Guessing Game   

    import random
    import time
    print("sayi tahmin oyununa hoşgeldin!z 1-100 arasında bir sayı tahmin edin")
    sayi = random.randint(1,100)
    tahmin_hakki = 5 
 
    while True:
    tahmin = int(input("tahmininiz: "))

    if tahmin == sayi:
        print("sayı sorgulanıyor... ")
        time.sleep(1)
        print("tebrlikler! Doğru Bildiniz")
        break
    elif tahmin > sayi:
        print("sayi sorgulanıyor... ")
        time.sleep(1)
        tahmin_hakki-=1
        print("Daha küçük bir sayı giriniz")
        print("kalan tahmin hakkı: ",tahmin_hakki)
    else:
        print("sayı sorgulanıyor... ")
        time.sleep(1)
        tahmin_hakki -=1
        print("daha büyük bir sayı giriniz")
        print("kalan tahmin hakkı: ", tahmin_hakki)
    if tahmin_hakki == 0:
        print("tahmin hakkınız bitmiştir")
        print("bilgisayarın tahmini",sayi)
        break
