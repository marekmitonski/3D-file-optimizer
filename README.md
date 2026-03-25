# 3D-file-optimizer

3D File Optimizer to lekkie, webowe narzędzie do optymalizacji plików OBJ z podglądem 3D w czasie rzeczywistym. Aplikacja działa w przeglądarce (bez backendu), więc pliki nigdy nie opuszczają Twojego komputera.

Funkcje
Wielometodowa kompresja siatek

redukcja precyzji współrzędnych (ucięcie miejsc po przecinku),

scalanie blisko położonych wierzchołków (vertex weld) ze skalą logarytmiczną,

uproszczanie siatki przez grid clustering.
Metody można dowolnie łączyć i sterować ich siłą osobnymi suwakami.

Podgląd przed/po kompresji

dwa panele: oryginał i model po kompresji,

współdzielona kamera i siatka – oba widoki zawsze pokazują tę samą scenę z tej samej perspektywy,

tryb wyświetlania siatki (wireframe) jako osobna warstwa, bez migotania (z-fighting).

Masowe przetwarzanie plików

wczytywanie wielu plików OBJ jednocześnie,

wczytywanie całych folderów z podkatalogami (rekurencyjnie),

lista plików z liczbą wierzchołków, trójkątów i statusem kompresji.

Eksport i formaty wyjściowe

zapis pojedynczego lub wszystkich plików do skompresowanego OBJ,

eksport do GLB (pojedynczo i masowo),

podgląd rozmiaru dla OBJ i GLB po kompresji.

Zachowanie struktury katalogów i nadpisywanie

zapis skompresowanych plików do wybranego folderu z zachowaniem struktury podkatalogów,

opcjonalne nadpisanie oryginalnych plików OBJ w źródłowym katalogu (z dodatkowym potwierdzeniem),

wsparcie File System Access API (Chrome/Edge).

Wygoda pracy

zapis ustawień kompresji (checkboxy + suwaki + tryb siatki) w localStorage,

po odświeżeniu przeglądarki ostatnia konfiguracja jest automatycznie przywracana,

wszystko w jednym pliku HTML – łatwe hostowanie na GitHub Pages lub dowolnym statycznym serwerze.

Możliwa jest integracja z pipeline’ami do gier, wizualizacji 3D lub webowych konfiguratorów, jako etap wstępnego „odchudzania” modeli przed wdrożeniem.