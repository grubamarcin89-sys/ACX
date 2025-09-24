# kalkulator.py
# Prosty kalkulator w Pythonie

def dodaj(a, b):
    return a + b

def odejmij(a, b):
    return a - b

def pomnoz(a, b):
    return a * b

def podziel(a, b):
    if b == 0:
        return "Błąd: dzielenie przez zero!"
    return a / b

print("=== Prosty Kalkulator ===")
print("Wybierz działanie:")
print("1. Dodawanie")
print("2. Odejmowanie")
print("3. Mnożenie")
print("4. Dzielenie")

wybor = input("Podaj numer operacji (1-4): ")

a = float(input("Podaj pierwszą liczbę: "))
b = float(input("Podaj drugą liczbę: "))

if wybor == "1":
    wynik = dodaj(a, b)
elif wybor == "2":
    wynik = odejmij(a, b)
elif wybor == "3":
    wynik = pomnoz(a, b)
elif wybor == "4":
    wynik = podziel(a, b)
else:
    wynik = "Nieprawidłowy wybór!"

print(f"Wynik: {wynik}")
