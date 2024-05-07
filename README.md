Metoda LZ77 to sposób kompresji danych, który zastępuje powtarzające się fragmenty danych symbolami wskazującymi na wcześniejsze wystąpienie tych danych. Proces kompresji odbywa się poprzez odczytanie pliku, skompresowanie danych za pomocą algorytmu LZ77 i zapisanie ich do pliku wyjściowego. Ten sam program umożliwia dekompresję pliku, przetwarzając skompresowane dane i odtwarzając oryginalny plik.

W implementacji używam języka C, operując na plikach tekstowych. Korzystam z 4-znakowego słownika i 4-znakowego bufora. Tworzę jedną długą listę typu char, w której pierwsze 8 elementów to bufor i słownik. Operacja ta kontynuowana jest, aż zostanie zapewnione co najmniej 5 wolnych miejsc.
