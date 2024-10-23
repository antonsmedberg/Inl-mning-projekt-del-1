# AI-Projekt: Objektigenkänning i Bilder

## Projektbeskrivning
Målet med detta projekt är att utveckla en avancerad maskininlärningsmodell som kan identifiera och lokalisera objekt, såsom människor och djur, i bilder. Modellen ska även kunna generera enkla och precisa bildbeskrivningar baserat på de identifierade objekten för att ge en helhetsförståelse av vad som händer i bilden.

## Datainsamling och Förberedelser
Jag har valt att använda **COCO-datasetet** (Common Objects in Context), ett välkänt dataset inom datorseende som innehåller annoterade bilder med objektkategorier och bildbeskrivningar. COCO är idealiskt då det erbjuder en bred variation av objekt och scenarier, vilket förbättrar modellens generaliseringsförmåga.

### Kvalitetskontroll av Dataset
För att säkerställa datasetets kvalitet och kompatibilitet kommer jag att:
- Inspektera och hantera eventuella null-värden och extrema värden för att undvika datafel.
- Validera att datatyperna är korrekt formaterade för modellträning.
- Rensa bort irrelevanta fält och konvertera data till lämpliga format som passar de algoritmer som används.

## Tekniker och Metoder
Projektet kombinerar flera tekniker för att lösa både klassificering, lokalisering och bildtextgenerering:

- **Convolutional Neural Networks (CNN)**: För att extrahera visuella funktioner och egenskaper från bilderna.
- **YOLOv5** eller **Faster R-CNN**: Används för precis och effektiv objektigenkänning och lokalisering.
- **Encoder-Decoder-arkitektur**: För bildtextgenerering, där en CNN fungerar som encoder och LSTM eller transformer-modeller används som decoder för att skapa bildbeskrivningar.

## Maskininlärningsstrategi
Eftersom datasetet är annoterat kommer jag att använda mig av **supervised learning**. Modellen tränas för att känna igen objekt och generera beskrivningar baserat på tidigare märkta exempel.

## Träningsplattform och Verktyg
Jag använder **PyTorch** som huvudsaklig träningsplattform på grund av dess flexibilitet och stöd för komplexa arkitekturer som YOLO och transformer-modeller. **Jupyter Notebook** kommer att användas för dataanalys, visualisering och experiment.

## Projektplan
1. **Datasetanalys**: Utforska datasetet och säkerställ att det är rent och korrekt formaterat.
2. **Dataaugmentation**: Använd tekniker som rotation, skalning och justering av ljus för att öka mångfalden och förbättra modellens generaliseringsförmåga.
3. **Modellutveckling**: Implementera en CNN-arkitektur i kombination med YOLO eller Faster R-CNN för objektigenkänning samt LSTM eller transformer-modeller för textgenerering.
4. **Hyperparameteroptimering**: Justera modellens hyperparametrar genom Grid Search eller Bayesian Optimization och utnyttja förtränade modeller när det är möjligt.
5. **Modellträning och Utvärdering**: Träna modellen på datasetet och utvärdera dess prestanda både för objektigenkänning och bildtextgenerering.
6. **Dokumentation**: Dokumentera projektets alla steg, insikter och resultat noggrant för att säkerställa spårbarhet och reproducibilitet.

## Nästa Steg
1. Utforska och visualisera datasetet i Jupyter Notebook för att förstå dess struktur och innehåll.
2. Förbered och standardisera data så att den är kompatibel med modellens inlärningskrav.
3. Bygg och testa träningspipelines för att genomföra den första omgången av modellträning och optimering.

## Mål och Lärandemål
Genom detta projekt vill jag:
- Lära mig att bygga och träna avancerade maskininlärningsmodeller för objektigenkänning.
- Förstå hur olika arkitekturer, såsom YOLO och transformers, kan kombineras för att skapa en komplett AI-lösning.
- Utveckla färdigheter inom hyperparameteroptimering och datahantering för att förbättra modellens prestanda och noggrannhet.
