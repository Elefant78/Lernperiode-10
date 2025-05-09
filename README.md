# Lernperiode-10

25.4 bis 27.6

## Grob-Planung

1. Welche Programmiersprache möchten Sie verwenden? Was denken Sie, wo Ihre Zeit und Übung am sinnvollsten ist? Ich denke es macht am meisten Sinn bei dem zu bleiben was ich schon kenne, deswegen werde ich C# benutzten
2. Welche Datenbank-Technologie möchten Sie üben? Fühlen Sie sich sicher mit SQL und möchten etwas Neues ausprobieren; oder möchten Sie sich weiter mit SQL beschäftigen? SQL, macht mir persönlich Spass, es würde vielleicht Sinn machen seine fähigkeiten zu diversifizieren, doch erst wenn man das eine gut genug kann.
3. Was wäre ein geeignetes Abschluss-Projekt? ich habe mir über legt ein Telephonebuch App zumachen, bei dem ich verschiedenste Nummer ein geben kann also auch ausländische, logischer weise soll auch der name drin stehen, sonst weiss man ja nicht wem die Nummer gehört.

## 25.4

Welche 3 *features* sind die wichtigsten Ihres Projektes? Wie können Sie die Machbarkeit dieser in jeweils 45' am einfachsten beweisen?

- [ ] *make or break feature* 1, Nummer eingeben:
- [ ] *make or break feature* 2, Nummer suchen:
- [ ] *make or break feature* 3, Nummer speicher:

Heute habe ich kurz und knapp raw programmiert, ich habe die neue Arbeitsmethode von Herrn Colic probiert, in der man 3 make or break features, quick and dirty programmiert, in meinem Fall wäre das das Speichernfeature, das Searchfeature und und das Eingabefeature. ich habe mit dem Speicher feature angefangen, da es auf mir den interessantes Eindruck bewirkt hat. Danach war die Searchfunktion dran. 

### Intern Nummern speichern


class Telefonbuch
{
    private Dictionary<string, string> kontakte = new Dictionary<string, string>();

    public void KontaktHinzufügen(string name, string nummer)
    {
        kontakte[name] = nummer;
    }

    public void AlleKontakteAnzeigen()
    {
        foreach (var eintrag in kontakte)
        {
            Console.WriteLine($"Name: {eintrag.Key}, Nummer: {eintrag.Value}");
        }
    }
}
### Search

public string NummerSuchen(string name)
{
    if (kontakte.ContainsKey(name))
    {
        return kontakte[name];
    }
    else
    {
        return "Nicht gefunden.";
    }
}


☝️ Vergessen Sie nicht, den Code von heute auf github hochzuladen. Ggf. bietet es sich an, für die Code-Schnipsel einen eigenen Ordner `exploration` zu erstellen.

## 2.5

Ausgehend von Ihren Erfahrungen vom 25.4, welche *features* brauchen noch mehr Recherche? (Sie können auch mehrere AP für ein *feature* aufwenden.)

- [X] Gui von App, entwerfen-->Grobe Struktur Offline-Arbeitspaket
- [X] Grundstruktur und Datenmodell erweitern; Klasse Kontakt erstellen mit Feldern: Name, Telefonnummer, Adresse, E-Mail
- [ ] Suche erweitern und verbessern; Mehrere Treffer anzeigen.
- [ ] Daten speichern & laden (Offline-Arbeit); Kontakte als SQL speichern und laden (System.Text.SQL).

Heute habe ich an weiter an dem Projekt gearbeitet, ich habe mich dazu entschieden mit Forms zuarbeiten. Ich finde es macht spass mit diesem Tool zu arbeiten und es ist abwechslungsreicher, da ich erstmals genug von python habe. Zurzeit bin ich an dem Verbinden mit einer SQL Datenbank dran. Es kommt eine Fehlermeldung bei mir, ich schaue mir es nächste Session an, wenn es nicht klappt melde ich mich bei Herrn Colic

<img width="550" alt="image" src="https://github.com/user-attachments/assets/116d83a1-046f-4fd4-8b60-d7377a284437" />

## 9.5

Planen Sie nun Ihr Projekt, sodass die *Kern-Funktionalität* in 3 Sitzungen realisiert ist. Schreiben Sie dazu zunächst 3 solche übergeordneten Kern-Funktionalitäten auf:

1. Kern-Funktionalität, Insert
2. Kern-Funktionalität, Delete
3. Kern-Funktionalität, Update

Diese Kern-Funktionalitäten brechen Sie nun in etwa 4 AP je herunter. Versuchen Sie jetzt bereits, auch die Sitzung vom 16.5 und 23.5 zu planen (im Wissen, dass Sie kleine Anpassungen an Ihrer Planung vornehmen können).

- [X] Eine Verbindung zwischen meinem Projekt und SQL herzustellen
- [X] Tabelles von Datenbank implementieren
- [ ] Insert button zum laufen bringen


Heute habe ich zum ersten Mal eine WinForms Applikation mit einem SQL server verbunden, dies hat mehr Zeit in anspruch genommen als gedacht. Es kamm öfters der Fehler, dass ich keine Berrechtigung habe, zum eine Verbindung zu einem SQL-Server und dem Winforms zu kreieren. Ich habe darauf hin ein Youtube-Tutorial geschaut wie man dieses Problem behebt, dies hat mich ziemlich viel Zeit gekostet. Die Erstellung des Insert Button ging vergleichsweise schnell, jeodch bekomme ich einen Fehler, wenn ich ein Element in E-mails einfüge. Für nächste woche ist das Ziel, diesen Fehler zu beheben.

<img width="412" alt ="Bild des Einfügeprozess" src ="https://github.com/user-attachments/assets/c14adf3c-8a62-41cd-b14e-f6876b8f74e1" />


<img width="412" alt="image" src="https://github.com/user-attachments/assets/dfebfdde-977c-4de0-af88-fb8e2a99a065" />

## 16.5

- [ ] ...
- [ ] ...
- [ ] ...
- [ ] ...

✍️ Heute habe ich... (50-100 Wörter)

☝️ Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 23.5

- [ ] ...
- [ ] ...
- [ ] ...
- [ ] ...

✍️ Heute habe ich... (50-100 Wörter)

☝️ Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 6.6

Ihr Projekt sollte nun alle Funktionalität haben, dass man es benutzen kann. Allerdings gibt es sicher noch Teile, welche "schöner" werden können: Layout, Code, Architektur... beschreiben Sie kurz den Stand Ihres Projekts, und leiten Sie daraus 6 solche "kosmetischen" AP für den 6.6 und den 13.6 ab.

- [ ] ...
- [ ] ...
- [ ] ...
- [ ] ...

✍️ Heute habe ich... (50-100 Wörter)

☝️ Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 13.6

- [ ] ...
- [ ] ...

✍️ Heute habe ich... (50-100 Wörter)

☝️ Vergessen Sie nicht, den Code von heute auf github hochzuladen.

## 20.6

Was fehlt Ihrem fertigen Projekt noch, um es auszuliefern? Reicht die Zeit für ein *nice-to-have feature*?

- [ ] ...

Bereiten Sie in den verbleibenden 2 AP Ihre Präsentation vor

- [ ] Materialien der Präsentation vorbereiten
- [ ] Präsentation üben

✍️ Heute habe ich... (50-100 Wörter)

☝️ Vergessen Sie nicht, die Unterlagen für Ihre Präsentation auf github hochzuladen.

## 27.6
