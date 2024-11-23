I denne oppgaven har jeg valgt å lage en RC-krets og koble denne til et 9V batteri på et breadboard. 
Uten å gjøre regningen kan vi allerede finne spenningen over kondensatoren ved hjelp av en differentiallikning 𝑅𝐶 ̇𝑣(𝑡) + 𝑣(𝑡) = 9, 𝑣(0) = 0. 
R her er en 10kOhms motstand og C er 100 μF kondesator, v(t) er spenningen over kondensatoren. Dette er en difflikning på formen 
τdt + x= k, hvor τ er RC, k er en konstant som referer til den "konstante spenningen" fra spenningskilden i dettte tilfelle 9V. Denne likningen har en løsning gitt ved x(t) = k+ [x(0)−k]e−t/τ. x(t) er v(t) og k = konstant spenning. Putter vi inn verdiene blir løsningen 9-9*e−t/τ. Denne bruker vi til å plotte teoretisk kurve.
Jeg har brukt denne til å plotte spenningen for teoretisk spenning og tatt egne målinger fra kretsen for målt spenning.
Bilde av plotten og punktene av målt data har jeg lagt til i repositoryen. På bilde ser vi klart at punktene ligger under den teoretiske kurven. PS: Det er unøyakitgheter i målingene fordi det kan hende jeg bomma litt med tiden siden det var et kort tidsintervall, men dette endrer ikke hvorfor punktene ligger lavere grafen. Det kan være flere grunner til hvorfor spenningen er lavere i praksis, men det er hovedsakelig tre: 

Spenningen vil fortsatt ha en eksponentiell graf, men med små forskjeller:
I batterier er det en indre motstand som kan påvirke kretser den kobles til. For å generere energi skjer det elektrokjemiske reaksjoner, disse har en motstand mot strømflyt. Temperaturen kan også påvirke farten på ionenes bevegelse. 
Andre ting som materialmotstand og motstand i elektrontransporten er også faktorer. Med dette observerer vi at:

1.Batteriets indre motstand kan redusere toppspenningen (f.eks., kanskje den aldri når helt 9V, men stopper på 8.8V).
  -Ved høy belastning kan spenningen stige litt saktere enn forventet, fordi batteriets indre motstand reduserer strømmen til kondensatoren.

2.Støy:
  -Målt spenning kan inneholde små variasjoner på grunn av følsomhet og evt variasjoner i batteriets ytelse.

3.Batteriets levetid:
  -Dette batteriet har jeg brukt i lang periode for andre fag. Ved lengre bruk vet vi at batteriet ikke vil ha maksimal ytelse og gi ut mindre strøm.
