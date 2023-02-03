 # Bar
  - Verbuchen von Gutscheine : 
    - Example Green Option :
      - Bestellen ↓ Bezahlen ↓ Rabatt ↓ Green Option 5 Euro ↓ Bar ↓ Cash 
  - No Post for Bar **ONLY FOR** hinterlegte Credit Card , Then auf zimmer Buchen *bedeutet* mann schreibt auf's Zimmer nur wenn eine hinterlegte CC da ist .
 
 
 #### Notes (Anmerkungen)
 - Rechnungen auf Zimmer _**IMMER**_ kopieren und in Meldeschein rein . *HERR STÖHR*
 - Rechnungen auf Zimmer , Es muss folgende Daten drauf sein : 
   - Name des Gastes . 
   - Zimmer Nummer . 
   - Unterschift des Gastes 
  -  **Hinweis** Nicht genutzter Wert des Gutscheins verfällt,Übersteigt der Gesamtwert der Bestellung den Wert des Gutscheins, wird dies noch Cash o.ä. verbucht . *HERR STÖHR* 
 
 # Check In
 - If No Show remains **more than One Night** , then we Have to post the First Night Cashiering ↓ billing  ↓ Post ↓ Room Revenue 7% ↓ Ok. and it should be posted in the Right Window . 
    - More than One Night means that the Nights in Reservation Mask is **NOT** Zero .
 - **Check-In A block of Group or a Group**
     - Reservations ↓ Blocks ↓ Search Group ↓ Double Click On found Group ↓ Group Opt. ↓ Check-In Group
 #### Notes (Anmerkungen)
 - BLAU bedeutet Inclusive Breakfast
 - Depo Betrag in Minus einfach einchecken
 - UDFCO3 can NOT be NULL => ROT schreiben Third field von Rm. Type .
 - By Agent : Berge & Meer Touristen , Zettel(Voucher) vom Gast nehmen und in Register Card einlegen.

 # Check Out

 #### Notes (Anmerkungen)
 - SZ and DEPO have to be checked out in Cashiering > Billing .
 - Erstmal TA und dann Auschecken ??? 

 # End Of Day (Tagesabschluss)

 # Formulate Bills (Rechnung Erstellen)
 - **Negative Posting (Reports Print Rechnung)**
     - Cashiering ↓ Cashier Func. ↓ Folio History ↓ First Date : -1 ↓ Second Date : leave as it is ↓ Room Nr. ↓ Search
 
 #### Notes (Anmerkungen)
 - When Routing, ask the guest about the Address  *HERR STÖHR*
 - By Check Out = Rechnung , By Payment = No Rechnung 
 - Rechnung wird **IMMER EINE NACHT VOR ABREISE ERSTELLT , NICHT VOHER** 
 
 # In House Guest
 - For Accompany Person NICHT cut new Key sondern Options ↓ **Key** ↓ **Cut Duplicate** , ansonsten werden alle Karten blockiert .
 - Room Move 2 Things should be in concern which is Traces for FO and Housekeeping : 
   - Search Room ↓ Options ↓ Room Move ↓ Move to Room + Reason  , and then Set the Traces : 
     - Search Room ↓ Options ↓ Traces ↓ Department Code should be FO and HSK and in Trace Text type that the person has changed from room to Room , and then set the Old room to Dirty : 
   - Rooms Management ↓ Housekeeping ↓ Housekeeping Management ↓ Type Room Nr. ↓ Search and set it to Dirty !
 - Putting charges of other rooms on a specific room : 
   - BEFORE Tagesabschluss Search The Room that its person NOT going to pay ↓ Options ↓ Routing ↓ Room NOT WINDOW ↓ Route to Room ↓ choose Room and the Transactions  ↓ Choose all or Transactions depending on
   - AFTER Tagesabschluss  : Cashiering ↓ Billing ↓ Search Room ↓ Double Click ↓ Right Click on Window Payment ↓ Transfer Transaction ↓ To Room ↓ Choose Room .
 - Breakfast : 
   - BEFORE tagesabschluss einfach unter Packages of the Profile
   - AFTER Tagesabschluss Cashiering ↓ Billing ↓ Search Room ↓ Post ↓ YES for 113 has no post flag on , Do you want to post anywhere ?  ↓  Code and choose what you want  ↓ under amount , put the amount  ↓ post … If he wants a Receipt then Click the Window where the Breakfast ist Posted and then Settlement . If he just would like to pay then ↓ Payment
   - Same Scenario with a Pet or whatever look at the above point except for pets before Tagesabschluss you look ↓ Fixed charges NOT profile .
 - To give Green Option *OR* to set a trace of it :  we don't Consider Arrival Date and Departure Date, and we ask the guest how many day's he doesn't want his room not to be cleaned and according to the amount of days he says we give an amount of Green Option .
    - By setting a trace Reservation Mask ↓ Item Inv ↓ New ↓ Item Code ↓ GO ↓ OK ↓ OK
      - and When you Click Save and Ok in the Main Reservation Mask , then come the Question *Inventory item GO has trace text attached. Create Trace?* ↓ Yes ↓ From Date: The First Day that the Room should not be cleaned ↓ To Date The last Day that the room should not be cleaned ↓ Ok .
  - We don't Reinstate NO SHOWS to avoid paying many **No Show Fees** .
  - **Traces** Setzen :
    - Late Check out ( Immer egal ob bevor oder nach TA )
    - Go 
    - Nacht verlaengern ( bleiber ) 
    - KU > under kostenuebernahmne Papers in KU FOLDER , you will fin something like **bitte senden Sie die rechnung an der email** , we have to take the KU paper and search for the gest in the In house Guest and set a trace to FO , and write down the Email address found in the paper .
  - **Alert** Setzen 
    - for information like **Bitte an HRewards Anmeldung Erinnern** , you will find that in the comments of the guest , and for that you have to set an alert !
      - Name of Guest > Options > Alert > Code : Gen > Area : Check out > Description : Bitte an HRewards Anmeldung erinnern > Ok > Ok .
  - **Post (Buchung)**
      - Post is da damit alles auf der Rechnung steht und rauskommt .
  - **Set a Membership for HRwards**
      - Profile ↓ Options ↓ Membership .

 # Payment Methods (Zahlungsarten)
 - Depo = VCC 
   - Types Of Guest in accordance with Payment :
     - KÜ : VCC, DEPO, Company mit CC, Company CityLdedger, PM
       - PM : is a Virtual Room where multiple guests come from a company continuously AND you can't make a Reciept Indiviually and it also means if an Individual Guest has a Wrong CC or didn't Pay etc .
       - Difference between PM and CityLedger KÜ is by CityLedger Reciepts are sent Individually to the Company and by PM every costs will be collected and pushed in the PM and One Reciept will be sent to the Company .
       - Difference between Company CC and Company CityLedger is by Company CC firstly Money and then Rechnungen , and Company CityLedger first the Rechnung and then The Money .
       - Difference between VCC and Depo is by VCC the guest pays the Platform Someday BUT the DEPO it's already paid before arrivals
         - Examples : 
           - RailAdventure = PM 
           - MEG = kÜ CC
           - Berge & Meer = CityLedger
           - Expedia, HRS, Hotelbeds = VCC
         - Notes :
           - CA or CL under Pay Type for PM , doesn't matter
           - CL is for CityLedger
     - SZ : CA, CC, EC
 - BO acto PM = KÜ
  - Before TA any cash taken should be in System by Cashiering ↓ Billing ↓ Payment , After TA it should be in System by Cashiering ↓ Billing ↓ Post and then Cashiering ↓ Billing ↓ Payment.
  - Credit Card Authorization Won't Work for a Checked in Guest Unless doing it in A manuel Way by editing Card Nr. and Expiration Date .. Example Breakfast after TA authorize !
  - Authorozation Rules : 
    - First Line : Pay Type ↓ CA , Auth Rule ↓ 5 , Amt/Pct ↓ 0
    - Other Lines depends on Reservation Methods (SZ,VCC etc ) : Pay Type ↓ CP, Auth Rule ↓ 1 , Amt/Pct ↓ 0 
    - If You put Auth Rule ↓ 1 then it means the Whole Fee(Beitrag Like nights,Breakfast etc) , and if you puth Auth Rule ↓ 5 and Amt/Pct ↓ 0 then it means you didn't block a Price from the Credit Card but you have ZUGRIFF auf the Credit Card .
 - Booking is *ALWAYS* Selbstzahler .
 - Room Paying can *also* be done from **Profile** not only Cashiering ↓ Billing ↓ Payment .
 - BO ac #203 *means* Kosten sind Übernommen von Room #203
 - We can Use *IF* we don't wanna print a Rechnung
 - Reservierungsmaske ↓ Options ↓ Credit Cards ↓ Authorization ↓ Additional Authorizathion *NOT MANUAL AUTHORIZATOIN* ↓ Additional Authorization Amount ↓ Type Amount *HERR STÖHR WAS RIGHT ABOUT SUSPICIOUS PEOPLE FROM THE BAR*
 - RG *means* Rechnung in Comments
 - *VERY IMPORTANT EXAMPLE OF A GUEST (HERR OVERKAMP) ON THE 30.01.2023,I WAS ALONE THAT DAY WITH CIARA , SHE WAS LATE-SHIFT AND I WAS A NIGHTY*
    - *Herr Overkamp war ein SZ for 4 NIGHTS WITHOUT BREAKFAST, und Wollte AND IN A SUDDEN HE DECIDED TO TAKE BREAKFAST FOR THE FOR NIGHT*  ***HOWTODO*** :
       - **FIRSTLY** set first Window : Pay Type ↓ CA , Auth Rule ↓ 5 , Amt/Pct ↓ 0
       - **SECOND** set *SECOND* window : Pay Type ↓ CP , Auth RUle ↓ 5 Amt/Pct ↓ *THE WHOLE AMOUNT FOR THE FOUR NIGHTS WHICH WAS 207 AND AS YOU SAY HERE WE SPECIFIED THE AMOUNT OF THE AUTHORIZED CARD*
       - **LASTLY** we make the payment of the Breakfast by *FIRSTLY* specifing that in the Reservierungsmaske ↓ Packages ↓ and pick up the Breakfast
           - **THEN** Cashiering ↓ Billing ↓ Payment ↓ and then we Put the amount of the *Breakfast for the whole 4 nights*

 # Reservations 
 - Reservations ↓ Update Reservation ↓ Arrival Date from … To … ↓ Advanced ↓ Search ↓ No Show
 - Reservation [ If Agent or Company or Irgendwas , we don't change anything in Reservierung , but we don't change Rate Code or Rate ] 
 - Registration Cards ↓ Individual, Blocks abhacken ↓ Blocks arrow down ↓ take Group Code Example CNIE221121 ↓ Miscellaneous ↓ Reports ↓ 24.012  ↓ Datum von morgen in Arrival Date , und Code unter Block Code. 
 - No Shows hat Preise von 90 % der Rate   *HERR STÖHR*
 - Green Option with Night Combination : Should be givin to someone who stays *2 NIGHTS == 3 DAYS*
 - BahnCards are for HRLevels
 - If there are **NO AVAILABLE** rooms in House then :
   - KostenÜbernahme zur anderen Hotel schicken
   - SZ sollen vor ort Bezahlen
 - *NOTE* Gruppe (DGRP) 
    - KÜ = erstellt mann **KEIN MELDESCHEIN**
    - PM = erstellt mann Meldescheine , wie normal .
 







  **Question Answers**
  
  - MEG ?
  - Add on ?
  - 1 Nacht nur , post oder nicht fuer letzte nacht bei reinstate ?
  - Pets nicht gebucht , gleich bezahlen oer CC Belasten ? 
  - Keine Reservierung , CIARA oder CC hinterlegen ?
  - Getraenke vom Bar , bei CC additional und betrag von Getraenke eingeben ?
  - Naechte verlaengern bei gaeste un gaeste die kein fruehstuck gebucht haben un wollen fruehstuck haben ?
  - nochmal gruppen melde schein durchgehen ?
  - nicht company address fuer rechnung durchgehen ?
  - nochmal traces fuer FO und HSK fuer reinstated no show durchgehen ?


  -1,2 GruppenList : 
    - MEG 
    - DGRP Minimum 5 *Person* Look in Arrival 
    - PM Minimum 5 *Person* Look inside Reservierungsmaske
  -3 Alle naechte Posten egal welche Zahlungsmittel 
  -4 kein CC = Gleich Zahlen , CC = fixed charges oder nach TA in Post .
  -5 CIARA
  -6 Ja
  -7 wenn die ueber uns gebucht haben wo bei der reservierungsmaske **HLINK CR** steht , ja kann mann normal verlaengern und dabei : 
     - eine Trace setzen fuer FO/HSK und als notiz schreibt man *anschlussbuchung* oder *bleiber* oder *Asb* .
     - wenn die ABER ueber uns nicht gebucht haben , dann muessen die eine neue buchung bei der webseite machen .
  - 
  **Question Answers**
  - Rate code nicht gefunden was machen ? und was mit dem betrag ? 
