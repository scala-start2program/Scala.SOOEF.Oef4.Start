# SOOEF : oefening 4
  
## Omschrijving  
  
Wij houden in dit programma een aantal eigendommen bij : vakantiehuisjes die kunnen verhuurd worden.   
Via het programma zal je dergelijke huisjes kunnen toevoegen, wijzigen en verwijderen.   
De verhuur zelf wordt hier (nog) niet in uitgewerkt.  

## WPF  
  
Je krijgt alle XAML code via deze repo.  
De event-handlers werden voor jou reeds aangemaakt.  
Bestudeer zelf aandachtig de namen van de verschillende controls.  

## Opdracht  

  * Maak een class library aan met de naam Scala.SOOEF.Oef4.Core  
  * Verwijder Class1 die automatisch werd aangemaakt  
  *
  * Voeg een nieuwe (entiteits) klasse toe met de naam **Vakantiehuis**  
  * Een vakantiehuis beschikt over volgende eigenschappen :   
    *  **Id** : string - full prop met enkel GET gedeelte  
    *  **Huisnaam** : string - full prop - lege waarden leveren een fout op  
    *  **Adres** : string - full prop  
    *  **Gemeente** : string - full prop  
    *  **PrijsPerNacht** : decimal - full prop - wanneer de waarde kleiner is dan 0, dan pas je deze automatisch aan naar 0  
    *  **MaxPersonen** byte - full prop - wanneer deze waarde groter is dan 12, dan pas je deze automatisch aan naar 12
  * Voorzie 2 constructors  
    * een argumentloze : in deze constructor zorg je er wel voor dat de eigenschap Id een unieke waarde krijgt (GUID of Global Unique Identifier).  
      Zo'n unieke waarde kan je als volgt genereren :    ... = Guid.NewGuid().ToString().  
    * een met evenveel argumenten als er eigenschappen zijn, behalve Id (dus huisnaam, adres, gemeente, prijsPerNacht en maxPersonen).  
      Vul met de argumenten de eigenschappen en genereer zelf een GUID waarde voor de eigenschap Id.
  * Overschrijf de ToString()-methode en toon de naam van het huis en de gemeente in de plaats.
  
  * Voeg een nieuwe (service) klasse toe met de naam **VakantiehuisService**   
  * Deze klasse heeft 1 (short) prop : **Vakantiehuizen** die een List is van Vakantiehuis-objecten  
  * De klasse heeft 1 (argumentloze) constructor  
  * Voorzie seeding (maak zelf een 4-tal huisjes aan)  
  * Voorzie methoden om vakantiehuisjes toe te voegen en vakantiehuisjes te verwijderen  
  * Zorg er tenslotte voor dat de huisjes aangeboden worden gesorteerd op naam van het huisje.  
  
  * In je WPF project voorzie je alles om deze vakantiehuisjes te beheren (afbeelden, toevoegen, wijzigen en verwijderen).  
    Maak hierbij verstandig gebruik van methoden wanneer je merkt dat bepaalde stukken code herhaald worden ...
  
