# Testy typu TLPT
O testach penetracyjnych pod kątem wyszukiwania zagrożeń (ang. threat-led penetration testing)

**Akty prawne**

1. [Rozporządzenie (EU) 2022/2554](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32022R2554#art_26) - DORA, w szczególności:

    - [Artykuł 26: Zaawansowane testowanie narzędzi, systemów i procesów ICT z wykorzystaniem TLPT](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32022R2554#art_26)
    - [Artykuł 27: Wymogi dotyczące testerów na potrzeby przeprowadzania TLPT](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32022R2554#art_27)

2. [Rozporządenie delegowane (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190) - doprecyzowujące kwestie, o których mowa w art. 26 pkt 11 [rozporządzenia (EU) 2022/2554](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32022R2554#art_26)

**TLPT a TIBER-EU**

Zgodnie z art. 3 pkt 17 [rozporządzenia (EU) 2022/2554](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32022R2554) (DORA), testy typu TLPT zdefiniowanse zostały jako:

*"testy penetracyjne pod kątem wyszukiwania zagrożeń (TLPT)” oznaczają ramy naśladujące taktykę, techniki i procedury stosowane w rzeczywistości przez agresorów uznanych za stanowiących rzeczywiste cyberzagrożenie, które zapewniają kontrolowane, dostosowane do konkretnych zagrożeń, oparte na analizie zagrożeń (red team) testy działających na bieżąco krytycznych systemów produkcji podmiotu finansowego;*

Zgodnie z [rozporządzeniem delegowanym (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190), testy typu TLPT są zgodne z ramami [TIBER-EU](https://www.ecb.europa.eu/paym/cyber-resilience/tiber-eu/html/index.en.html):

*Niniejsze rozporządzenie zostało opracowane zgodnie z ramami TIBER-EU i odzwierciedla metodykę, proces i strukturę testów penetracyjnych pod kątem wyszukiwania zagrożeń (TLPT) opisanych w TIBER-EU. Podmioty finansowe podlegające obowiązkowi przeprowadzania TLPT mogą odwoływać się do ram TIBER-EU lub krajowych przepisów wdrażających te ramy i stosować te ramy lub przepisy, o ile są one zgodne z wymogami określonymi w art. 26 i 27 rozporządzenia (UE) 2022/2554 oraz w niniejszym rozporządzeniu. Wyznaczenie jednego organu publicznego w sektorze finansowym odpowiedzialnego na poziomie krajowym za kwestie związane z TLPT zgodnie z art. 26 ust. 9 rozporządzenia (UE) 2022/2554 powinno pozostawać bez uszczerbku dla kompetencji właściwych organów w zakresie nadzoru nad niektórymi podmiotami finansowymi powierzonych na poziomie Unii – zgodnie z art. 46 tego rozporządzenia – organom takim jak na przykład Europejski Bank Centralny w odniesieniu do istotnych instytucji kredytowych, które to organy należy uznać za właściwe w kwestiach związanych z TLPT. W przypadku gdy tylko niektóre zadania związane z TLPT są przekazywane innemu organowi krajowemu w sektorze finansowym na podstawie art. 26 ust. 10 rozporządzenia (UE) 2022/2554, organem właściwym dla zadań związanych z TLPT, które nie zostały przekazane, powinien nadal być właściwy organ w odniesieniu do danego podmiotu finansowego wskazany w art. 46 tego rozporządzenia.*

## Analiza zagrożeń

Zgodnie z art. 3 pkt 15 [rozporządzenia (EU) 2022/2554](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32022R2554) (DORA), analiza zagrożeń na potrzeby testów typu TLPT zdefiniowana została jako:

*„analiza zagrożeń” oznacza informacje, które zostały zagregowane, przekształcone, przeanalizowane, zinterpretowane lub wzbogacone w celu zapewnienia niezbędnego kontekstu na potrzeby podejmowania decyzji i umożliwienia odpowiedniego i wystarczającego zrozumienia w celu złagodzenia skutków incydentu związanego z ICT lub cyberzagrożenia, w tym informacje dotyczące technicznych szczegółów cyberataku, osób odpowiedzialnych za atak oraz ich sposobu działania i motywacji;*

Dodatkowo art. 1 pkt 10 [rozporządzenia delegowanego (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190) definiuje dostawcę analizy zagrożeń jako:

*„dostawca analizy zagrożeń” oznacza ekspertów, z którymi podmiot finansowy zawiera umowę na każde TLPT i którzy są zewnętrzni w stosunku do podmiotu finansowego i dostawców usług ICT wewnątrz grupy, jeśli tacy istnieją, oraz którzy gromadzą i analizują ukierunkowane informacje z analizy zagrożeń istotne dla podmiotów finansowych w zakresie konkretnego procesu TLPT oraz opracowują odpowiednie i realistyczne scenariusze zagrożeń;*

W szczególności należy zauważyć, iż dostawca taki jest zawsze zewnętrzny w stosunku do testowanego podmiotu finansowego. [Rozporządzenie delegowane (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190) tak opisuje rolę dostawcy analizy zagrożeń:

*Aby zapewnić testerom informacje potrzebne do symulacji rzeczywistego i realistycznego ataku na działające na bieżąco systemy podmiotu finansowego stanowiące podstawę jego krytycznych lub istotnych funkcji, dostawca analizy zagrożeń powinien gromadzić dane lub informacje dotyczące co najmniej dwóch kluczowych obszarów zainteresowania:*
 - *celów, poprzez zidentyfikowanie potencjalnych powierzchni ataku w całym podmiocie finansowym,*
 - *zagrożeń, poprzez zidentyfikowanie odnośnych agresorów i prawdopodobnych scenariuszy zagrożeń.*

*W celu zapewnienia, aby dostawca analizy zagrożeń uwzględnił zagrożenia istotne dla podmiotu finansowego, testerzy, zespół typu control team i kierownicy testów powinni udzielić mu informacji zwrotnej na temat projektu sprawozdania z analizy zagrożeń. Jako punkt odniesienia dla krajowego krajobrazu zagrożeń dostawca analizy zagrożeń może wykorzystać ogólny krajobraz zagrożeń stworzony przez organ ds. TLPT dla sektora finansowego danego państwa członkowskiego, o ile jest on dostępny. Jak wynika ze stosowania ram TIBER-EU, proces gromadzenia informacji na potrzeby analizy zagrożeń trwa zazwyczaj około 4 tygodni.*

### Wymogi formalne dla dostawcy analizy zagrożeń

Ogólne wymagania jakie powinień spełniać taki dostawca zostały przedstawione w art. 27 pkt 1 [rozporządzenia (EU) 2022/2554](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32022R2554) (DORA):

*a) są najbardziej odpowiedni do tego zadania i cieszą się największą renomą;*

*b) posiadają zdolności techniczne i organizacyjne oraz wykazują się szczególną wiedzą fachową w zakresie analizy zagrożeń, testów penetracyjnych i testów z udziałem zespołów typu red team;*

*c) posiadają certyfikat wydany przez jednostkę akredytującą w państwie członkowskim lub przystąpili do formalnych kodeksów postępowania lub ram etycznych;*

*d) przedstawiają niezależne zapewnienie lub sprawozdanie z audytu dotyczące należytego zarządzania ryzykiem związanym z przeprowadzaniem TLPT, w tym należytej ochrony poufnych informacji podmiotu finansowego i dochodzenia roszczeń z tytułu ryzyka biznesowego podmiotu finansowego;*

*e) są należycie i w pełni objęci odpowiednimi ubezpieczeniami od odpowiedzialności cywilnej z tytułu wykonywania zawodu, w tym od ryzyka uchybień i zaniedbań.*

Bardziej konkretne wymagania, które powinien spełniać taki dostawca zawiera art. 7 pkt 1 lit. a)–c) [rozporządzenia delegowanego (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190#art_7):

*a) dostawca analizy zagrożeń i zewnętrzni testerzy dostarczyli zespołowi typu control team szczegółowy życiorys i kopie certyfikatów, które zgodnie z uznanymi standardami rynkowymi stanowią poświadczenie ich odpowiedniości do wykonywania powierzonych im zadań;*

*b) dostawca analizy zagrożeń i zewnętrzni testerzy byli należycie i w pełni objęci odpowiednimi ubezpieczeniami od odpowiedzialności cywilnej z tytułu wykonywania zawodu, w tym od ryzyka uchybień i zaniedbań;*

*c) dostawca analizy zagrożeń przedstawił co najmniej trzy rekomendacje z powierzonych mu poprzednio zadań w zakresie testów penetracyjnych i testów z udziałem zespołu typu red team;*

[Rozporządzenie delegowane (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190#art_7)) określa, także wymogi dla personelu dostawcy analizy zagrożeń ( art. 7 pkt 1 lit. e):

*(i) obejmował co najmniej kierownika z co najmniej pięcioletnim doświadczeniem w zakresie analizy zagrożeń oraz co najmniej jednego dodatkowego członka z co najmniej dwuletnim doświadczeniem w zakresie analizy zagrożeń;*

*(ii) wykazywał się szerokim zakresem i odpowiednim poziomem wiedzy i umiejętności zawodowych, obejmujących:*

  *1) taktyki, techniki i procedury gromadzenia danych wywiadowczych;*
  *2) wiedzę geopolityczną, techniczną i sektorową;*
  *3) odpowiednie umiejętności komunikacyjne umożliwiające jasne przedstawianie wyników jego pracy i składanie sprawozdań na ten temat;*

*(iii) brał łącznie udział w co najmniej trzech wcześniejszych zadaniach związanych z analizą zagrożeń w kontekście testów penetracyjnych i testów z udziałem zespołu typu red team;*

*(iv) nie wykonywał jednocześnie żadnych zadań zespołu typu blue team ani innych usług, które mogą stanowić konflikt interesów w odniesieniu do podmiotu finansowego, zewnętrznego dostawcy usług ICT lub dostawcy usług ICT wewnątrz grupy zaangażowanych w TLPT, do których personel ten został przydzielony;*

*(v) był oddzielony od personelu tego samego dostawcy TLPT, który zapewnia testerów zewnętrznych na potrzeby tych samych TLPT, i nie podlegał temu personelowi;*

Analizując powyższe, warto w szczególności zauważyć iż:

1. Etap analizy zagrożeń trwa (średnio) około 4 tygodni (wynika to z doświadczeń zdobytych podczas przeprowadzania testów w modelu TIBER-EU);
2. Analiza zagrożeń powinna być przeprowadzana przez zespół w składzie przynajmniej 2 analityków: kierownik (min. 5 lat doświadczenia), młodszy analityk (min. 2 lata doświadczenia) o odpowiednich kwalifikacjach;
3. Dostawcy analizy zagrożeń przedstawiają niezależne zapewnienie lub sprawozdanie z audytu dotyczące należytego zarządzania ryzykiem związanym z przeprowadzaniem TLPT - na przykład może to być zrealizowane poprzez: kwestionariusz oceny bezpieczeństwa, gotowość do poddania się "audytowi drugiej strony", posiadanie certyfikatu na zgodność np. z ISO 27001, itd.;
4. Dostawca analizy zagrożeń powinien być ubezpieczony od odpowiedzialności cywilnej z tytułu wykonywania zawodu, w tym od ryzyka uchybień i zaniedbań;
5. Personel dostawcy analizy zagrożeń powinien być wolny od konfliktów interesów (np. nie pracować wcześniej jako członek blue team'u w testowanej organizacji lub nie pełnić jednocześnie roli analityka zagrożeń i testera).

### Ogólny krajobraz zagrożeń (GTL)

[Rozporządzenie delegowane (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190#art_10)) rekomenduje (art. 10 pkt 1) aby dostawca analizy zagrożeń jako punkt wyjścia dla swojej analizy wykorzystał ogólny krajobraz zagrożeń dla sektora finansowego, jeśli takowy jest dostępny:

*... W przypadku gdy organ ds. TLPT stworzył ogólny krajobraz zagrożeń dla sektora finansowego państwa członkowskiego, dostawca analizy zagrożeń może wykorzystać ten krajobraz jako punkt odniesienia dla krajowego krajobrazu zagrożeń. ...*

W Polsce organem ds. TLPT został [Urząd Komisji Nadzoru Finansowego (UKNF)](https://www.knf.gov.pl/), który od 2025 roku publikuje taki dokument:

[Krajobraz cyberzagrożeń w polskim sektorze finansowym (2026)](https://cebrf.knf.gov.pl/images/GTL%202026.pdf)

[Krajobraz cyberzagrożeń w polskim sektorze finansowym (2025)](https://cebrf.knf.gov.pl/images/GTL_2025_FINAL.pdf)

Warto, także zapoznać się z:

[Polski Rynek Finansowy w obliczu zagrożeń](https://www.knf.gov.pl/knf/pl/komponenty/img/Raport_Roczny_CSIRT_KNF_2025-23_03_97516.pdf)

### Rola i zadania dostawców analizy zagrożeń w testach TLPT

[Art. 10 pkt rozporządzenia delegowanego (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190#art_10) zawiera dalsze wytyczne dla dostawcy analizy zagrożeń.

[Załącznik III rozporządzenia delegowanego (EU) 2025/1190](https://eur-lex.europa.eu/legal-content/PL/TXT/?uri=CELEX:32025R1190#anx_III) opisuje wymaganą treść sprawozdania z ukierunkowanej analizy zagrożeń.

## Skróty i definicje

| Definicja | Wyjaśnienie |
| :--- | :--- |
| TLPT | testy penetracyjne pod kątem wyszukiwania zagrożeń (TLPT)” oznaczają ramy naśladujące taktykę, techniki i procedury stosowane w rzeczywistości przez agresorów uznanych za stanowiących rzeczywiste cyberzagrożenie, które zapewniają kontrolowane, dostosowane do konkretnych zagrożeń, oparte na analizie zagrożeń (red team) testy działających na bieżąco krytycznych systemów produkcji podmiotu finansowego - zgodnie z art. 3 pkt 17 rozporządzenia (EU) 2022/2554 (DORA) |
| Analiza zagrożeń | oznacza informacje, które zostały zagregowane, przekształcone, przeanalizowane, zinterpretowane lub wzbogacone w celu zapewnienia niezbędnego kontekstu na potrzeby podejmowania decyzji i umożliwienia odpowiedniego i wystarczającego zrozumienia w celu złagodzenia skutków incydentu związanego z ICT lub cyberzagrożenia, w tym informacje dotyczące technicznych szczegółów cyberataku, osób odpowiedzialnych za atak oraz ich sposobu działania i motywacji - zgodnie z art. 3 pkt 15 rozporządzenia (EU) 2022/2554 (DORA) |
| Dostawca analizy zagrożeń | oznacza ekspertów, z którymi podmiot finansowy zawiera umowę na każde TLPT i którzy są zewnętrzni w stosunku do podmiotu finansowego i dostawców usług ICT wewnątrz grupy, jeśli tacy istnieją, oraz którzy gromadzą i analizują ukierunkowane informacje z analizy zagrożeń istotne dla podmiotów finansowych w zakresie konkretnego procesu TLPT oraz opracowują odpowiednie i realistyczne scenariusze zagrożeń - zgodnie z art. 1 pkt 10 rozporządzenia delegowanego (EU) 2025/1190 |

