# PeShopSystem

PetShop je web aplikacija za upravljanje prodavnicom ljubimaca, razvijena na .NET platformi koristeći višeslojnu arhitekturu. Sistem omogućava korisnicima da se registruju i prijave putem JWT autentifikacije, nakon čega dobijaju pristup svim funkcionalnostima. Kroz intuitivan interfejs korisnik može pregledati listu ljubimaca, pretraživati ih po imenu ili rasi, dodavati nove, izmjenjivati postojeće i brisati ih, kao i upravljati kategorijama i dobavljačima. 

Aplikacija je izgrađena po principu razdvajanja odgovornosti — Entities sloj definiše modele podataka, DAL sloj komunicira sa SQL Server bazom podataka kroz parametrizovane SQL upite, BusinessLayer obrađuje poslovnu logiku i vraća standardizovane rezultate, API projekat izlaže REST endpointe testirane kroz Swagger, a WebApp je Blazor Server aplikacija koja pruža interaktivan korisnički interfejs. 

Sigurnost sistema je osigurana BCrypt hashiranjem lozinki i JWT tokenima koji se čuvaju u localStorage browsera, dok je kvalitet poslovne logike potvrđen jediničnim testovima pisanim po AAA principu uz korišćenje Mock objekata.
