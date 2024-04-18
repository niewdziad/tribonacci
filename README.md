# tribonacci
#
def tribonacci(length=8, signature=(0, 1, 1)):: Definiuje funkcję tribonacci, która przyjmuje dwa argumenty: length (długość ciągu do wygenerowania) i signature (początkowy ciąg). Domyślne wartości to 8 dla length i (0, 1, 1) dla signature.

if length == 0:: Sprawdza, czy length jest równe 0. Jeśli tak, zwraca pustą listę, ponieważ nie ma nic do wygenerowania.

elif length <= 3:: Sprawdza, czy length jest mniejsze lub równe 3. Jeśli tak, zwraca listę składającą się z pierwszych length elementów sygnatury.

result = list(signature): Tworzy listę result na podstawie podanej sygnatury, aby móc ją zmieniać.

for i in range(3, length):: Rozpoczyna pętlę, zaczynając od 3, ponieważ pierwsze trzy liczby są już w result. Pętla będzie iterować od 3 do length - 1.

next_num = sum(result[-3:]): Oblicza następną liczbę Tribonacciego przez dodanie ostatnich trzech liczb z listy result.

result.append(next_num): Dodaje obliczoną następną liczbę Tribonacci do listy result.

return result: Zwraca wygenerowany ciąg liczb Tribonacci.

print(tribonacci()): Wywołuje funkcję tribonacci bez podawania argumentów, co spowoduje wygenerowanie domyślnego ciągu liczb Tribonacci o długości 8 i wydrukowanie go.