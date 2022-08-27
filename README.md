# openHAB-Alexa-Speechcons
Using openHAB and the [Amazon Echo Control Binding](https://www.openhab.org/addons/bindings/amazonechocontrol/) to run german [speechcons](https://developer.amazon.com/en-US/docs/alexa/custom-skills/speechcon-reference-interjections-german.html).

## Items

For each speechcon we need to create a `Switch` item. If this `Switch` item changed to `ON` a rule with an speechcon will be triggered.

```
Group Amazon_EchoDot_Redewendungen "Redewendungen" <text>

Switch Amazon_EchoDot_Redewendung_Ach_du_liebe_Zeit "Ach du liebe Zeit" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Aber_Hallo "Aber hallo" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Aber_sicher "Aber sicher" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Abrakadabra "Abrakadabra" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ach "Ach" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ach_du_gruene_Neune "Ach du grüne Neune" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ach_du_meine_Guete "Ach du meine Güte" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ach_ja "Ach ja" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ach_so "Ach so" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Achje "Achje" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Achtung "Achtung" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ade "Ade" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ah "Ah" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Aha "Aha" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Aehm "Ähm" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ahoi "Ahoi" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Alles_klar "Alles klar" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Aloha "Aloha" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Als_ob "Als ob" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Argh "Argh" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Arrivederci "Arrivederci" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Aso "Aso" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Au "Au" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Au_weia "Au weia" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Aua "Aua" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Autsch "Autsch" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bazinga "Bazinga" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bingo "Bingo" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bis_bald "Bis bald" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bis_dann "Bis dann" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bla "Bla" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Boing "Boing" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bon_Appetit "Bon Appetit" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bon_Voyage "Bon Voyage" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bonjour "Bonjour" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bravo "Bravo" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Brumm "Brumm" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Buh "Buh" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Buhu "Buhu" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bumm "Bumm" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Bzz "Bzz" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Da_lachen_ja_die_Huehner "Da lachen ja die Hühner" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ding_Dong "Ding Dong" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Dito "Dito" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Donner_und_Doria "Donner und Doria" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Donnerwetter "Donnerwetter" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ebenso "Ebenso" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_En_Garde "En Garde" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ey "Ey" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Geh_nur "Geh nur" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Gemach "Gemach" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Genug "Genug" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Gesundheit "Gesundheit" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Gott_im_Himmel "Gott im Himmel" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Gruess_Gott "Grüß Gott" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Gute_Reise "Gute Reise" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Guten_Appetit "Guten Appetit" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hach_ja "hach ja" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Halleluja "Halleluja" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hals_und_Beinbruch "Hals- und Beinbruch" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Halt "Halt" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Haende_hoch "Hände hoch" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Heiliger_Strohsack "Heiliger Strohsack" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Heisa "Heisa" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hey "Hey" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hihi "Hihi" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hipp_Hipp_Hurra "Hipp, Hipp, Hurra" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hoert_hoert "Hört, hört" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hue "Hü" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Huea "Hüa" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Huch "Huch" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Huhu "Huhu" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hui "Hui" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Hurra "Hurra" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ich_glaube_ich_bin_im_Kino "Ich glaube ich bin im Kino" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ich_glaub_mein_Schwein_pfeifft "Ich glaub mein Schwein pfeifft" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ich_glaub_mich_knutsch_ein_Elch "Ich glaub mich knutscht ein Elch" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ich_glaub_mich_laust_der_Affe "Ich glaub mich laust der Affe" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ich_glaub_mich_tritt_ein_Pferd "Ich glaub mich tritt ein Pferd" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Igitt "Igitt" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Iiieh "Iiieh" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ist_nicht_dein_Ernst "Ist nicht dein Ernst" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Japp "Japp" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Jawohl "Jawohl" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Jo "Jo" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Juhu "Juhu" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Kein_Kommentar "Kein Kommentar" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Keine_Ursache "Keine Ursache" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Kikeriki "Kikeriki" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Klar "Klar" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Klick_Klack "Klick, Klack" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Kopf_hoch "Kopf hoch" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Kuckuck "Kuckuck" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Lass_es_dir_schmecken "Lass es dir schmecken" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Lecker "Lecker" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Los "Los" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Mach_s_gut "Mach's gut" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Mahlzeit "Mahlzeit" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Mamma_mia "Mamma mia" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Mann_ueber_Board "Mann über Board" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Manometer "Manometer" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Mazel_tov "Mazel tov" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Mein_Gott "Mein Gott" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Merci "Merci" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Miau "Miau" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Moin "Moin" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Muh "Muh" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Na_klar "Na klar" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Na_sieh_mal_einer_an "Na sieh mal einer an" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Na_und "Na und?" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Na "Na?" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Naja "Naja" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Nanu "Nanu" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ne "Ne" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Nee "Nee" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Nichts_da "Nichts da" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Nix_da "Nix da" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Noe "Nö" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Null_problemo "Null problemo" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Obacht "Obacht" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Och "Och" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Oh_Mann "Oh Mann" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Oh_mein_Gott "Oh mein Gott" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Oh_my_god "Oh my god" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Oh_nein "Oh nein" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Oh_oh "Oh, oh" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ohne_Scheiss "Ohne Scheiß" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Oink "Oink" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Oje "Oje" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Okey_dokey "Okey, dokey" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Ooh_la_la "Ooh la la" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Pfui "Pfui" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Piep "Piep" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Plop "Plop" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Plumps "Plumps" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Prima "Prima" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Prosit "Prosit" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Prost "Prost" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Puff "Puff" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Puh "Puh" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Pustekuchen "Pustekuchen" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Schachmatt "Schachmatt" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Schade "Scahde" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Schau_an "Schau an" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Sesam_oeffne_dich "Sesam öffne dich!" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Seufz "Seufz" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Sieh_an "Sieh an!" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Siehe_da "Siehe da!" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Siehste "Siehste!" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Spoileralarm "Spoileralarm" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Stimmt "Stimmt" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Super "Super" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Supi "Supi" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Suesses_oder_Saures "Süßes oder Saures?" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Tada "Tada" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Tatsaechlich "Tatsächlich" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Tick_Tack "Tick, tack" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Tja "Tja" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Touche "Touché" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Tschoe "Tschö" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Tuerlich "Türlich" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Tut "Tut" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Uff "Uff" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Verdammt "Verdammt" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Verflixt "Verflixt" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Viel_Glueck "Viel Glück" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Voila "Voilá" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Von_wegen "Von wegen" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Vorsicht "Vorsicht" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_War_nur_ein_Scherz "War nur ein Scherz" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Was_zur_Hoelle "Was zur Hölle?" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Weh_mir "Weh mir" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Wehe "Wehe" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Wie_du_meinst "Wie du meinst" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Willkommen "Willkommen" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Wow "Wow" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Wuff "Wuff" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Yay "Yay" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Zugabe "Zugabe" <text> (Amazon_EchoDot_Redewendungen)
Switch Amazon_EchoDot_Redewendung_Zum_Wohl "Zum Wohl" <text> (Amazon_EchoDot_Redewendungen)
```

## Rules

Additionally to the speechcons items you have to create an `<textToSpeech_item>`. Therefore you need to configure the [Amazon Echo Control Binding](https://www.openhab.org/addons/bindings/amazonechocontrol/) and an `Amazo Echo` product. At least you have to create an `<textToSpeech_item>` item which are used for text to speech (tts).

```
rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ach_du_liebe_Zeit"
when
    Item Amazon_EchoDot_Speechcon_Ach_du_liebe_Zeit changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ach du liebe zeit</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Aber_Hallo"
when
    Item Amazon_EchoDot_Speechcon_Aber_Hallo changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">aber hallo</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Aber_sicher"
when
    Item Amazon_EchoDot_Speechcon_Aber_sicher changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">aber sicher</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Abrakadabra"
when
    Item Amazon_EchoDot_Speechcon_Abrakadabra changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">abrakadabra</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ach"
when
    Item Amazon_EchoDot_Speechcon_Ach changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ach</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ach_du_gruene_Neune"
when
    Item Amazon_EchoDot_Speechcon_Ach_du_gruene_Neune changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ach du grüne neune</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ach_du_meine_Guete"
when
    Item Amazon_EchoDot_Speechcon_Ach_du_meine_Guete changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ach du meine güte</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ach_ja"
when
    Item Amazon_EchoDot_Speechcon_Ach_ja changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ach ja</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ach_so"
when
    Item Amazon_EchoDot_Speechcon_Ach_so changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ach so</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Achje"
when
    Item Amazon_EchoDot_Speechcon_Achje changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">achje</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Achtung"
when
    Item Amazon_EchoDot_Speechcon_Achtung changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">achtung</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ade"
when
    Item Amazon_EchoDot_Speechcon_Ade changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ade</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ah"
when
    Item Amazon_EchoDot_Speechcon_Ah changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ah</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Aha"
when
    Item Amazon_EchoDot_Speechcon_Aha changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">aha</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Aehm"
when
    Item Amazon_EchoDot_Speechcon_Aehm changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ähm</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ahoi"
when
    Item Amazon_EchoDot_Speechcon_Ahoi changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ahoi</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Alles_klar"
when
    Item Amazon_EchoDot_Speechcon_Alles_klar changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">alles klar</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Aloha"
when
    Item Amazon_EchoDot_Speechcon_Aloha changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">aloha</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Als_ob"
when
    Item Amazon_EchoDot_Speechcon_Als_ob changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">als ob</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Argh"
when
    Item Amazon_EchoDot_Speechcon_Argh changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">argh</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Arrivederci"
when
    Item Amazon_EchoDot_Speechcon_Arrivederci changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">arrivederci</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Aso"
when
    Item Amazon_EchoDot_Speechcon_Aso changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">aso</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Au"
when
    Item Amazon_EchoDot_Speechcon_Au changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">au</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Au_weia"
when
    Item Amazon_EchoDot_Speechcon_Au_weia changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">au weia</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Aua"
when
    Item Amazon_EchoDot_Speechcon_Aua changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">aua</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Autsch"
when
    Item Amazon_EchoDot_Speechcon_Autsch changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">autsch</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bazinga"
when
    Item Amazon_EchoDot_Speechcon_Bazinga changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bazinga</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bingo"
when
    Item Amazon_EchoDot_Speechcon_Bingo changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bingo</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bis_bald"
when
    Item Amazon_EchoDot_Speechcon_Bis_bald changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bis bald</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bis_dann"
when
    Item Amazon_EchoDot_Speechcon_Bis_dann changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bis dann</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bla"
when
    Item Amazon_EchoDot_Speechcon_Bla changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bla</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Boing"
when
    Item Amazon_EchoDot_Speechcon_Boing changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">boing</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bon_Appetit"
when
    Item Amazon_EchoDot_Speechcon_Bon_Appetit changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bon appetit</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bon_Voyage"
when
    Item Amazon_EchoDot_Speechcon_Bon_Voyage changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bon voyage</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bonjour"
when
    Item Amazon_EchoDot_Speechcon_Bonjour changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bonjour</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bravo"
when
    Item Amazon_EchoDot_Speechcon_Bravo changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bravo</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Brumm"
when
    Item Amazon_EchoDot_Speechcon_Brumm changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">brumm</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Buh"
when
    Item Amazon_EchoDot_Speechcon_Buh changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">buh</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Buhu"
when
    Item Amazon_EchoDot_Speechcon_Buhu changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">buhu</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bumm"
when
    Item Amazon_EchoDot_Speechcon_Bumm changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bumm</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Bzz"
when
    Item Amazon_EchoDot_Speechcon_Bzz changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">bzz</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Da_lachen_ja_die_Huehner"
when
    Item Amazon_EchoDot_Speechcon_Da_lachen_ja_die_Huehner changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">da lachen ja die hühner</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ding_Dong"
when
    Item Amazon_EchoDot_Speechcon_Ding_Dong changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ding dong</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Dito"
when
    Item Amazon_EchoDot_Speechcon_Dito changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">dito</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Donner_und_Doria"
when
    Item Amazon_EchoDot_Speechcon_Donner_und_Doria changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">donner und doria</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Donnerwetter"
when
    Item Amazon_EchoDot_Speechcon_Donnerwetter changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">donnerwetter</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ebenso"
when
    Item Amazon_EchoDot_Speechcon_Ebenso changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ebenso</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_En_Garde"
when
    Item Amazon_EchoDot_Speechcon_En_Garde changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">en garde</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ey"
when
    Item Amazon_EchoDot_Speechcon_Ey changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ey</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Geh_nur"
when
    Item Amazon_EchoDot_Speechcon_Geh_nur changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">geh nur</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Gemach"
when
    Item Amazon_EchoDot_Speechcon_Gemach changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">gemach</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Genug"
when
    Item Amazon_EchoDot_Speechcon_Genug changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">genug</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Gesundheit"
when
    Item Amazon_EchoDot_Speechcon_Gesundheit changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">gesundheit</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Gott_im_Himmel"
when
    Item Amazon_EchoDot_Speechcon_Gott_im_Himmel changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">gott im himmel</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Gruess_Gott"
when
    Item Amazon_EchoDot_Speechcon_Gruess_Gott changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">grüß gott</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Gute_Reise"
when
    Item Amazon_EchoDot_Speechcon_Gute_Reise changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">gute reise</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Guten_Appetit"
when
    Item Amazon_EchoDot_Speechcon_Guten_Appetit changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">guten appetit</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hach_ja"
when
    Item Amazon_EchoDot_Speechcon_Hach_ja changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hach ja</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Halleluja"
when
    Item Amazon_EchoDot_Speechcon_Halleluja changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">halleluja</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hals_und_Beinbruch"
when
    Item Amazon_EchoDot_Speechcon_Hals_und_Beinbruch changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hals und beinbruch</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Halt"
when
    Item Amazon_EchoDot_Speechcon_Halt changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">halt</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Haende_hoch"
when
    Item Amazon_EchoDot_Speechcon_Haende_hoch changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hände hoch</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Heiliger_Strohsack"
when
    Item Amazon_EchoDot_Speechcon_Heiliger_Strohsack changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">heiliger strohsack</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Heisa"
when
    Item Amazon_EchoDot_Speechcon_Heisa changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">heisa</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hey"
when
    Item Amazon_EchoDot_Speechcon_Hey changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hey</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hihi"
when
    Item Amazon_EchoDot_Speechcon_Hihi changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hihi</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hipp_Hipp_Hurra"
when
    Item Amazon_EchoDot_Speechcon_Hipp_Hipp_Hurra changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hipp hipp hurra</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hoert_hoert"
when
    Item Amazon_EchoDot_Speechcon_Hoert_hoert changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hört hört</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hue"
when
    Item Amazon_EchoDot_Speechcon_Hue changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hü</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Huea"
when
    Item Amazon_EchoDot_Speechcon_Huea changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hüa</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Huch"
when
    Item Amazon_EchoDot_Speechcon_Huch changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">huch</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Huhu"
when
    Item Amazon_EchoDot_Speechcon_Huhu changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">huhu</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hui"
when
    Item Amazon_EchoDot_Speechcon_Hui changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hui</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Hurra"
when
    Item Amazon_EchoDot_Speechcon_Hurra changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">hurra</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ich_glaube_ich_bin_im_Kino"
when
    Item Amazon_EchoDot_Speechcon_Ich_glaube_ich_bin_im_Kino changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ich glaub ich bin im kino</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ich_glaub_mein_Schwein_pfeifft"
when
    Item Amazon_EchoDot_Speechcon_Ich_glaub_mein_Schwein_pfeifft changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ich glaub mein schwein pfeift</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ich_glaub_mich_knutsch_ein_Elch"
when
    Item Amazon_EchoDot_Speechcon_Ich_glaub_mich_knutsch_ein_Elch changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ich glaub mich knutscht ein elch</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ich_glaub_mich_laust_der_Affe"
when
    Item Amazon_EchoDot_Speechcon_Ich_glaub_mich_laust_der_Affe changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ich glaub mich laust der affe</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ich_glaub_mich_tritt_ein_Pferd"
when
    Item Amazon_EchoDot_Speechcon_Ich_glaub_mich_tritt_ein_Pferd changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ich glaub mich tritt ein pferd</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Igitt"
when
    Item Amazon_EchoDot_Speechcon_Igitt changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">igitt</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Iiieh"
when
    Item Amazon_EchoDot_Speechcon_Iiieh changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">iiieh</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ist_nicht_dein_Ernst"
when
    Item Amazon_EchoDot_Speechcon_Ist_nicht_dein_Ernst changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ist nicht dein ernst</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Japp"
when
    Item Amazon_EchoDot_Speechcon_Japp changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">japp</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Jawohl"
when
    Item Amazon_EchoDot_Speechcon_Jawohl changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">jawohl</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Jo"
when
    Item Amazon_EchoDot_Speechcon_Jo changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">jo</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Juhu"
when
    Item Amazon_EchoDot_Speechcon_Juhu changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">juhu</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Kein_Kommentar"
when
    Item Amazon_EchoDot_Speechcon_Kein_Kommentar changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">kein kommentar</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Keine_Ursache"
when
    Item Amazon_EchoDot_Speechcon_Keine_Ursache changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">keine ursache</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Kikeriki"
when
    Item Amazon_EchoDot_Speechcon_Kikeriki changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">kikeriki</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Klar"
when
    Item Amazon_EchoDot_Speechcon_Klar changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">klar</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Klick_Klack"
when
    Item Amazon_EchoDot_Speechcon_Klick_Klack changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">klick klack</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Kopf_hoch"
when
    Item Amazon_EchoDot_Speechcon_Kopf_hoch changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">kopf hoch</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Kuckuck"
when
    Item Amazon_EchoDot_Speechcon_Kuckuck changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">kuckuck</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Lass_es_dir_schmecken"
when
    Item Amazon_EchoDot_Speechcon_Lass_es_dir_schmecken changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">lass es dir schmecken</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Lecker"
when
    Item Amazon_EchoDot_Speechcon_Lecker changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">lecker</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Los"
when
    Item Amazon_EchoDot_Speechcon_Los changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">los</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Mach_s_gut"
when
    Item Amazon_EchoDot_Speechcon_Mach_s_gut changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">mach\'s gut</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Mahlzeit"
when
    Item Amazon_EchoDot_Speechcon_Mahlzeit changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">mahlzeit</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Mamma_mia"
when
    Item Amazon_EchoDot_Speechcon_Mamma_mia changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">mamma mia</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Mann_ueber_Board"
when
    Item Amazon_EchoDot_Speechcon_Mann_ueber_Board changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">mann über bord</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Manometer"
when
    Item Amazon_EchoDot_Speechcon_Manometer changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">manometer</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Mazel_tov"
when
    Item Amazon_EchoDot_Speechcon_Mazel_tov changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">mazel tov</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Mein_Gott"
when
    Item Amazon_EchoDot_Speechcon_Mein_Gott changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">mein gott</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Merci"
when
    Item Amazon_EchoDot_Speechcon_Merci changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">merci</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Miau"
when
    Item Amazon_EchoDot_Speechcon_Miau changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">miau</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Moin"
when
    Item Amazon_EchoDot_Speechcon_Moin changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">moin</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Muh"
when
    Item Amazon_EchoDot_Speechcon_Muh changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">muh</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Na_klar"
when
    Item Amazon_EchoDot_Speechcon_Na_klar changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">na klar</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Na_sieh_mal_einer_an"
when
    Item Amazon_EchoDot_Speechcon_Na_sieh_mal_einer_an changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">na sieh mal einer an</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Na_und"
when
    Item Amazon_EchoDot_Speechcon_Na_und changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">na und?</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Na"
when
    Item Amazon_EchoDot_Speechcon_Na changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">na?</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Naja"
when
    Item Amazon_EchoDot_Speechcon_Naja changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">naja</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Nanu"
when
    Item Amazon_EchoDot_Speechcon_Nanu changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">nanu?</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ne"
when
    Item Amazon_EchoDot_Speechcon_Ne changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ne</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Nee"
when
    Item Amazon_EchoDot_Speechcon_Nee changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">nee</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Nichts_da"
when
    Item Amazon_EchoDot_Speechcon_Nichts_da changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">nichts da</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Nix_da"
when
    Item Amazon_EchoDot_Speechcon_Nix_da changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">nix da</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Noe"
when
    Item Amazon_EchoDot_Speechcon_Noe changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">nö</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Null_problemo"
when
    Item Amazon_EchoDot_Speechcon_Null_problemo changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">null problemo</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Obacht"
when
    Item Amazon_EchoDot_Speechcon_Obacht changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">obacht</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Och"
when
    Item Amazon_EchoDot_Speechcon_Och changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">och</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Oh_Mann"
when
    Item Amazon_EchoDot_Speechcon_Oh_Mann changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">oh mann</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Oh_mein_Gott"
when
    Item Amazon_EchoDot_Speechcon_Oh_mein_Gott changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">oh mein gott</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Oh_my_god"
when
    Item Amazon_EchoDot_Speechcon_Oh_my_god changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">oh my god</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Oh_nein"
when
    Item Amazon_EchoDot_Speechcon_Oh_nein changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">oh nein</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Oh_oh"
when
    Item Amazon_EchoDot_Speechcon_Oh_oh changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">oh oh</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ohne_Scheiss"
when
    Item Amazon_EchoDot_Speechcon_Ohne_Scheiss changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ohne scheiß</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Oink"
when
    Item Amazon_EchoDot_Speechcon_Oink changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">oink</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Oje"
when
    Item Amazon_EchoDot_Speechcon_Oje changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">oje</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Okey_dokey"
when
    Item Amazon_EchoDot_Speechcon_Okey_dokey changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">okey dokey</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Ooh_la_la"
when
    Item Amazon_EchoDot_Speechcon_Ooh_la_la changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">ooh la la</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Pfui"
when
    Item Amazon_EchoDot_Speechcon_Pfui changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">pfui</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Piep"
when
    Item Amazon_EchoDot_Speechcon_Piep changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">piep</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Plop"
when
    Item Amazon_EchoDot_Speechcon_Plop changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">plop</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Plumps"
when
    Item Amazon_EchoDot_Speechcon_Plumps changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">plumps</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Prima"
when
    Item Amazon_EchoDot_Speechcon_Prima changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">prima</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Prosit"
when
    Item Amazon_EchoDot_Speechcon_Prosit changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">prosit</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Prost"
when
    Item Amazon_EchoDot_Speechcon_Prost changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">prost</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Puff"
when
    Item Amazon_EchoDot_Speechcon_Puff changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">puff</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Puh"
when
    Item Amazon_EchoDot_Speechcon_Puh changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">puh</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_PusteMultimedian"
when
    Item Amazon_EchoDot_Speechcon_PusteMultimedian changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">pusteMultimedian</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Schachmatt"
when
    Item Amazon_EchoDot_Speechcon_Schachmatt changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">schachmatt</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Schade"
when
    Item Amazon_EchoDot_Speechcon_Schade changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">schade</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Schau_an"
when
    Item Amazon_EchoDot_Speechcon_Schau_an changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">schau an</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Sesam_oeffne_dich"
when
    Item Amazon_EchoDot_Speechcon_Sesam_oeffne_dich changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">sesam öffne dich</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Seufz"
when
    Item Amazon_EchoDot_Speechcon_Seufz changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">seufz</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Sieh_an"
when
    Item Amazon_EchoDot_Speechcon_Sieh_an changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">sieh an</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Siehe_da"
when
    Item Amazon_EchoDot_Speechcon_Siehe_da changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">siehe da</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Siehste"
when
    Item Amazon_EchoDot_Speechcon_Siehste changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">siehste?</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Spoileralarm"
when
    Item Amazon_EchoDot_Speechcon_Spoileralarm changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">spoileralarm</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Stimmt"
when
    Item Amazon_EchoDot_Speechcon_Stimmt changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">stimmt</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Super"
when
    Item Amazon_EchoDot_Speechcon_Super changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">super</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Supi"
when
    Item Amazon_EchoDot_Speechcon_Supi changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">supi</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Suesses_oder_Saures"
when
    Item Amazon_EchoDot_Speechcon_Suesses_oder_Saures changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">süßes oder saures</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Tada"
when
    Item Amazon_EchoDot_Speechcon_Tada changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">tada</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Tatsaechlich"
when
    Item Amazon_EchoDot_Speechcon_Tatsaechlich changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">tatsächlich</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Tick_Tack"
when
    Item Amazon_EchoDot_Speechcon_Tick_Tack changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">tick tack</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Tja"
when
    Item Amazon_EchoDot_Speechcon_Tja changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">tja</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Touche"
when
    Item Amazon_EchoDot_Speechcon_Touche changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">touche</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Tschoe"
when
    Item Amazon_EchoDot_Speechcon_Tschoe changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">tschö</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Tuerlich"
when
    Item Amazon_EchoDot_Speechcon_Tuerlich changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">türlich</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Tut"
when
    Item Amazon_EchoDot_Speechcon_Tut changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">tut</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Uff"
when
    Item Amazon_EchoDot_Speechcon_Uff changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">uff</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Verdammt"
when
    Item Amazon_EchoDot_Speechcon_Verdammt changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">verdammt</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Verflixt"
when
    Item Amazon_EchoDot_Speechcon_Verflixt changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">verflixt</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Viel_Glueck"
when
    Item Amazon_EchoDot_Speechcon_Viel_Glueck changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">viel glück</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Voila"
when
    Item Amazon_EchoDot_Speechcon_Voila changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">voila</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Von_wegen"
when
    Item Amazon_EchoDot_Speechcon_Von_wegen changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">von wegen</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Vorsicht"
when
    Item Amazon_EchoDot_Speechcon_Vorsicht changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">vorsicht</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_War_nur_ein_Scherz"
when
    Item Amazon_EchoDot_Speechcon_War_nur_ein_Scherz changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">war nur ein scherz</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Was_zur_Hoelle"
when
    Item Amazon_EchoDot_Speechcon_Was_zur_Hoelle changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">was zur hölle</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Weh_mir"
when
    Item Amazon_EchoDot_Speechcon_Weh_mir changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">weh mir</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Wehe"
when
    Item Amazon_EchoDot_Speechcon_Wehe changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">wehe</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Wie_du_meinst"
when
    Item Amazon_EchoDot_Speechcon_Wie_du_meinst changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">wie du meinst</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Willkommen"
when
    Item Amazon_EchoDot_Speechcon_Willkommen changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">willkommen</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Wow"
when
    Item Amazon_EchoDot_Speechcon_Wow changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">wow</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Wuff"
when
    Item Amazon_EchoDot_Speechcon_Wuff changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">wuff</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Yay"
when
    Item Amazon_EchoDot_Speechcon_Yay changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">yay</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Zugabe"
when
    Item Amazon_EchoDot_Speechcon_Zugabe changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">zugabe</say-as>.</speak>')
end

rule "Running Alexa Speechcon  Amazon_EchoDot_Speechcon_Zum_Wohl"
when
    Item Amazon_EchoDot_Speechcon_Zum_Wohl changed to ON
then
    <textToSpeech_item>.sendCommand('<speak><say-as interpret-as="interjection">zum wohl</say-as>.</speak>')
end

rule "Fixing gMultimedia_Amazon_EchoDot_Speechcon Switch OFF"
when
    Member of gMultimedia_Amazon_EchoDot_Speechcon changed from OFF to ON
then
    createTimer(now.plusNanos(1000000000), [ |
        //sendCommand(triggeringItem.name.split("_").get(0).toString, OFF)
        triggeringItem.sendCommand(OFF)
    ])
end
```

## Sitemaps

At least you have to add your items to the sitemap:

```
Text label="Redewendungen" {
    Switch item=Amazon_EchoDot_Redewendung_Ach_du_liebe_Zeit
    Switch item=Amazon_EchoDot_Redewendung_Aber_Hallo
    Switch item=Amazon_EchoDot_Redewendung_Aber_sicher
    Switch item=Amazon_EchoDot_Redewendung_Abrakadabra
    Switch item=Amazon_EchoDot_Redewendung_Ach
    Switch item=Amazon_EchoDot_Redewendung_Ach_du_gruene_Neune
    Switch item=Amazon_EchoDot_Redewendung_Ach_du_meine_Guete
    Switch item=Amazon_EchoDot_Redewendung_Ach_ja
    Switch item=Amazon_EchoDot_Redewendung_Ach_so
    Switch item=Amazon_EchoDot_Redewendung_Achje
    Switch item=Amazon_EchoDot_Redewendung_Achtung
    Switch item=Amazon_EchoDot_Redewendung_Ade
    Switch item=Amazon_EchoDot_Redewendung_Ah
    Switch item=Amazon_EchoDot_Redewendung_Aha
    Switch item=Amazon_EchoDot_Redewendung_Aehm
    Switch item=Amazon_EchoDot_Redewendung_Ahoi
    Switch item=Amazon_EchoDot_Redewendung_Alles_klar
    Switch item=Amazon_EchoDot_Redewendung_Aloha
    Switch item=Amazon_EchoDot_Redewendung_Als_ob
    Switch item=Amazon_EchoDot_Redewendung_Argh
    Switch item=Amazon_EchoDot_Redewendung_Arrivederci
    Switch item=Amazon_EchoDot_Redewendung_Aso
    Switch item=Amazon_EchoDot_Redewendung_Au
    Switch item=Amazon_EchoDot_Redewendung_Au_weia
    Switch item=Amazon_EchoDot_Redewendung_Aua
    Switch item=Amazon_EchoDot_Redewendung_Autsch
    Switch item=Amazon_EchoDot_Redewendung_Bazinga
    Switch item=Amazon_EchoDot_Redewendung_Bingo
    Switch item=Amazon_EchoDot_Redewendung_Bis_bald
    Switch item=Amazon_EchoDot_Redewendung_Bis_dann
    Switch item=Amazon_EchoDot_Redewendung_Bla
    Switch item=Amazon_EchoDot_Redewendung_Boing
    Switch item=Amazon_EchoDot_Redewendung_Bon_Appetit
    Switch item=Amazon_EchoDot_Redewendung_Bon_Voyage
    Switch item=Amazon_EchoDot_Redewendung_Bonjour
    Switch item=Amazon_EchoDot_Redewendung_Bravo
    Switch item=Amazon_EchoDot_Redewendung_Brumm
    Switch item=Amazon_EchoDot_Redewendung_Buh
    Switch item=Amazon_EchoDot_Redewendung_Buhu
    Switch item=Amazon_EchoDot_Redewendung_Bumm
    Switch item=Amazon_EchoDot_Redewendung_Bzz
    Switch item=Amazon_EchoDot_Redewendung_Da_lachen_ja_die_Huehner
    Switch item=Amazon_EchoDot_Redewendung_Ding_Dong
    Switch item=Amazon_EchoDot_Redewendung_Dito
    Switch item=Amazon_EchoDot_Redewendung_Donner_und_Doria
    Switch item=Amazon_EchoDot_Redewendung_Donnerwetter
    Switch item=Amazon_EchoDot_Redewendung_Ebenso
    Switch item=Amazon_EchoDot_Redewendung_En_Garde
    Switch item=Amazon_EchoDot_Redewendung_Ey
    Switch item=Amazon_EchoDot_Redewendung_Geh_nur
    Switch item=Amazon_EchoDot_Redewendung_Gemach
    Switch item=Amazon_EchoDot_Redewendung_Genug
    Switch item=Amazon_EchoDot_Redewendung_Gesundheit
    Switch item=Amazon_EchoDot_Redewendung_Gott_im_Himmel
    Switch item=Amazon_EchoDot_Redewendung_Gruess_Gott
    Switch item=Amazon_EchoDot_Redewendung_Gute_Reise
    Switch item=Amazon_EchoDot_Redewendung_Guten_Appetit
    Switch item=Amazon_EchoDot_Redewendung_Hach_ja
    Switch item=Amazon_EchoDot_Redewendung_Halleluja
    Switch item=Amazon_EchoDot_Redewendung_Hals_und_Beinbruch
    Switch item=Amazon_EchoDot_Redewendung_Halt
    Switch item=Amazon_EchoDot_Redewendung_Haende_hoch
    Switch item=Amazon_EchoDot_Redewendung_Heiliger_Strohsack
    Switch item=Amazon_EchoDot_Redewendung_Heisa
    Switch item=Amazon_EchoDot_Redewendung_Hey
    Switch item=Amazon_EchoDot_Redewendung_Hihi
    Switch item=Amazon_EchoDot_Redewendung_Hipp_Hipp_Hurra
    Switch item=Amazon_EchoDot_Redewendung_Hoert_hoert
    Switch item=Amazon_EchoDot_Redewendung_Hue
    Switch item=Amazon_EchoDot_Redewendung_Huea
    Switch item=Amazon_EchoDot_Redewendung_Huch
    Switch item=Amazon_EchoDot_Redewendung_Huhu
    Switch item=Amazon_EchoDot_Redewendung_Hui
    Switch item=Amazon_EchoDot_Redewendung_Hurra
    Switch item=Amazon_EchoDot_Redewendung_Ich_glaube_ich_bin_im_Kino
    Switch item=Amazon_EchoDot_Redewendung_Ich_glaub_mein_Schwein_pfeifft
    Switch item=Amazon_EchoDot_Redewendung_Ich_glaub_mich_knutsch_ein_Elch
    Switch item=Amazon_EchoDot_Redewendung_Ich_glaub_mich_laust_der_Affe
    Switch item=Amazon_EchoDot_Redewendung_Ich_glaub_mich_tritt_ein_Pferd
    Switch item=Amazon_EchoDot_Redewendung_Igitt
    Switch item=Amazon_EchoDot_Redewendung_Iiieh
    Switch item=Amazon_EchoDot_Redewendung_Ist_nicht_dein_Ernst
    Switch item=Amazon_EchoDot_Redewendung_Japp
    Switch item=Amazon_EchoDot_Redewendung_Jawohl
    Switch item=Amazon_EchoDot_Redewendung_Jo
    Switch item=Amazon_EchoDot_Redewendung_Juhu
    Switch item=Amazon_EchoDot_Redewendung_Kein_Kommentar
    Switch item=Amazon_EchoDot_Redewendung_Keine_Ursache
    Switch item=Amazon_EchoDot_Redewendung_Kikeriki
    Switch item=Amazon_EchoDot_Redewendung_Klar
    Switch item=Amazon_EchoDot_Redewendung_Klick_Klack
    Switch item=Amazon_EchoDot_Redewendung_Kopf_hoch
    Switch item=Amazon_EchoDot_Redewendung_Kuckuck
    Switch item=Amazon_EchoDot_Redewendung_Lass_es_dir_schmecken
    Switch item=Amazon_EchoDot_Redewendung_Lecker
    Switch item=Amazon_EchoDot_Redewendung_Los
    Switch item=Amazon_EchoDot_Redewendung_Mach_s_gut
    Switch item=Amazon_EchoDot_Redewendung_Mahlzeit
    Switch item=Amazon_EchoDot_Redewendung_Mamma_mia
    Switch item=Amazon_EchoDot_Redewendung_Mann_ueber_Board
    Switch item=Amazon_EchoDot_Redewendung_Manometer
    Switch item=Amazon_EchoDot_Redewendung_Mazel_tov
    Switch item=Amazon_EchoDot_Redewendung_Mein_Gott
    Switch item=Amazon_EchoDot_Redewendung_Merci
    Switch item=Amazon_EchoDot_Redewendung_Miau
    Switch item=Amazon_EchoDot_Redewendung_Moin
    Switch item=Amazon_EchoDot_Redewendung_Muh
    Switch item=Amazon_EchoDot_Redewendung_Na_klar
    Switch item=Amazon_EchoDot_Redewendung_Na_sieh_mal_einer_an
    Switch item=Amazon_EchoDot_Redewendung_Na_und
    Switch item=Amazon_EchoDot_Redewendung_Na
    Switch item=Amazon_EchoDot_Redewendung_Naja
    Switch item=Amazon_EchoDot_Redewendung_Nanu
    Switch item=Amazon_EchoDot_Redewendung_Ne
    Switch item=Amazon_EchoDot_Redewendung_Nee
    Switch item=Amazon_EchoDot_Redewendung_Nichts_da
    Switch item=Amazon_EchoDot_Redewendung_Nix_da
    Switch item=Amazon_EchoDot_Redewendung_Noe
    Switch item=Amazon_EchoDot_Redewendung_Null_problemo
    Switch item=Amazon_EchoDot_Redewendung_Obacht
    Switch item=Amazon_EchoDot_Redewendung_Och
    Switch item=Amazon_EchoDot_Redewendung_Oh_Mann
    Switch item=Amazon_EchoDot_Redewendung_Oh_mein_Gott
    Switch item=Amazon_EchoDot_Redewendung_Oh_my_god
    Switch item=Amazon_EchoDot_Redewendung_Oh_nein
    Switch item=Amazon_EchoDot_Redewendung_Oh_oh
    Switch item=Amazon_EchoDot_Redewendung_Ohne_Scheiss
    Switch item=Amazon_EchoDot_Redewendung_Oink
    Switch item=Amazon_EchoDot_Redewendung_Oje
    Switch item=Amazon_EchoDot_Redewendung_Okey_dokey
    Switch item=Amazon_EchoDot_Redewendung_Ooh_la_la
    Switch item=Amazon_EchoDot_Redewendung_Pfui
    Switch item=Amazon_EchoDot_Redewendung_Piep
    Switch item=Amazon_EchoDot_Redewendung_Plop
    Switch item=Amazon_EchoDot_Redewendung_Plumps
    Switch item=Amazon_EchoDot_Redewendung_Prima
    Switch item=Amazon_EchoDot_Redewendung_Prosit
    Switch item=Amazon_EchoDot_Redewendung_Prost
    Switch item=Amazon_EchoDot_Redewendung_Puff
    Switch item=Amazon_EchoDot_Redewendung_Puh
    Switch item=Amazon_EchoDot_Redewendung_Pustekuchen
    Switch item=Amazon_EchoDot_Redewendung_Schachmatt
    Switch item=Amazon_EchoDot_Redewendung_Schade
    Switch item=Amazon_EchoDot_Redewendung_Schau_an
    Switch item=Amazon_EchoDot_Redewendung_Sesam_oeffne_dich
    Switch item=Amazon_EchoDot_Redewendung_Seufz
    Switch item=Amazon_EchoDot_Redewendung_Sieh_an
    Switch item=Amazon_EchoDot_Redewendung_Siehe_da
    Switch item=Amazon_EchoDot_Redewendung_Siehste
    Switch item=Amazon_EchoDot_Redewendung_Spoileralarm
    Switch item=Amazon_EchoDot_Redewendung_Stimmt
    Switch item=Amazon_EchoDot_Redewendung_Super
    Switch item=Amazon_EchoDot_Redewendung_Supi
    Switch item=Amazon_EchoDot_Redewendung_Suesses_oder_Saures
    Switch item=Amazon_EchoDot_Redewendung_Tada
    Switch item=Amazon_EchoDot_Redewendung_Tatsaechlich
    Switch item=Amazon_EchoDot_Redewendung_Tick_Tack
    Switch item=Amazon_EchoDot_Redewendung_Tja
    Switch item=Amazon_EchoDot_Redewendung_Touche
    Switch item=Amazon_EchoDot_Redewendung_Tschoe
    Switch item=Amazon_EchoDot_Redewendung_Tuerlich
    Switch item=Amazon_EchoDot_Redewendung_Tut
    Switch item=Amazon_EchoDot_Redewendung_Uff
    Switch item=Amazon_EchoDot_Redewendung_Verdammt
    Switch item=Amazon_EchoDot_Redewendung_Verflixt
    Switch item=Amazon_EchoDot_Redewendung_Viel_Glueck
    Switch item=Amazon_EchoDot_Redewendung_Voila
    Switch item=Amazon_EchoDot_Redewendung_Von_wegen
    Switch item=Amazon_EchoDot_Redewendung_Vorsicht
    Switch item=Amazon_EchoDot_Redewendung_War_nur_ein_Scherz
    Switch item=Amazon_EchoDot_Redewendung_Was_zur_Hoelle
    Switch item=Amazon_EchoDot_Redewendung_Weh_mir
    Switch item=Amazon_EchoDot_Redewendung_Wehe
    Switch item=Amazon_EchoDot_Redewendung_Wie_du_meinst
    Switch item=Amazon_EchoDot_Redewendung_Willkommen
    Switch item=Amazon_EchoDot_Redewendung_Wow
    Switch item=Amazon_EchoDot_Redewendung_Wuff
    Switch item=Amazon_EchoDot_Redewendung_Yay
    Switch item=Amazon_EchoDot_Redewendung_Zugabe
    Switch item=Amazon_EchoDot_Redewendung_Zum_Wohl
}
```
