# PD

1. API jeb lietojumprogrammu saskarne ir noteikumu kopums, kas ļauj dažādām programmatūrām savstarpēji sazināties. Tas nodrošina veidu, kā viena programmatūra var pieprasīt un saņemt informāciju no citas programmatūras, tādējādi ļaujot dažādām sistēmām un servisiem integrēties un strādāt kopā.

2. PHP valodā mainīgos var deklarēt, izmantojot dollāra zīmi ($) un vēlamo mainīgā nosaukumu. Piemēram: $mainigais = "vērtība";
  
3. Laravel ir PHP programmēšanas valodas pamatā balstīta tīmekļa lietojumu izstrādes rīks, kas piedāvā iebūvētus risinājumus dažādām vajadzībām, ieskaitot maršrutēšanu, datu bāzu integrāciju, lietotāja autentifikāciju un daudz ko citu. Laravel lieto Model-View-Controller (MVC) arhitektūras modeli, kas ir ļoti populārs tīmekļa lietojumu izstrādē.
Laravel izmanto šādu arhitektūru:
Routes (Maršruti): Maršruti definē, kuri pieprasījumi tiek nosūtīti uz kuru kontrolieri. Maršrutēšana var būt vienkārša (piemēram, /home) vai arī tā var ietvert parametrus vai pat URI sapludināšanu.
Controllers (Kontrolieri): Kontrolieri ir atbildīgi par apstrādi, kas notiek, kad tiek saņemts konkrēts maršruts. Viņi atbild par datu sagatavošanu un pārvaldību, kā arī par to, kāda informācija tiek atgriezta skatam vai nosūtīta klientam.
Models (Modeļi): Modeļi ir datu struktūras, kas tiek izmantotas, lai sazinātos ar datu bāzi. Tie piedāvā veidu, kā ērti veikt datu ieguvi, ievietošanu, atjaunināšanu un dzēšanu, izmantojot Laravel iebūvētās Eloquent ORM iespējas.
Views (Skati): Skati ir klienta puse, kas attēlo informāciju lietotājam. Tie parasti satur HTML kopā ar PHP kodu vai Blade šablonu dzinēju, kas ļauj izveidot dinamiskus skatus, ievietojot datus tieši no kontrolieriem.

4. ORM ir objektu-relāciju kartēšanas (Object-Relational Mapping) sistēma, kas ļauj attēlot objektu orientētu programmēšanas valodu datu modeli relāciju datubāzē. Tas nodrošina programmētājiem abstrakciju no konkrētas datu bāzes sistēmas, ļaujot strādāt ar datiem, izmantojot objektu orientētu pieeju, nevis tieši rakstot SQL pieprasījumus.
Šeit ir daži iemesli, kāpēc var izmantot ORM tīra SQL vietā:
Objektu Orientēta Pieeja: ORM ļauj programmētājiem strādāt ar datiem, izmantojot objektu orientētu pieeju, kas padara kodu lasāmāku un vieglāk uztveramu. Tā vietā, lai manipulētu ar tabulām un rindām, programmētāji var strādāt ar objektiem un metodēm.
Mazāk Atkārtošanās: ORM ļauj atkārtoti izmantot kodu, jo datu bāzes operācijas tiek abstrahētas un tiek definētas vienreiz, kas var būt izmantojams visā aplikācijā. Tas samazina kodu dublēšanos un uzlabo uzturējamību.
Platformas Neatkarība: Izmantojot ORM, jūs varat viegli mainīt datu bāzes platformu, jo ORM aprūpējas ar datu bāzes konkrētās sintakses pielāgošanu. Tas nozīmē, ka jūs varat migrēt no vienas datu bāzes platformas uz citu, nemainot lielāko daļu kodu.
Drošība: ORM bieži vien piedāvā iebūvētas drošības funkcijas, piemēram, parametrizētas pieprasījumu veidošanu, kas pasargā no SQL injekcijas uzbrukumiem.
Veiktspējas Optimizācija: Lai gan ORM var būt mazliet lēnāks nekā tieša SQL izmantošana, lielākā daļa ORM sistēmu piedāvā veiktspējas optimizācijas iespējas, kas palīdz samazināt darbību laiku un resursu izmantošanu.

5.
use App\Models\User;

$users = User::where('rating', '>', 4)->get();
