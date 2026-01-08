# Deutschlandatlas-API

Der [Deutschlandatlas](https://www.deutschlandatlas.bund.de/DE/Home/home_node.html) ist ein Internetangebot, herausgegeben vom Bundesministerium für Wohnen, Stadtentwicklung und Bauwesen. Dort finden sich interaktive Karten zu gleichwertigen Lebensverhältnissen auf Grundlage aktueller verfügbarer Daten.
Informationen zu allen [Indikatoren](https://www.deutschlandatlas.bund.de/DE/Service/Downloads/Indikatoren_Deutschlandatlas.html) sowie aktuelle Daten in [tabellarischer Form](https://www.deutschlandatlas.bund.de/DE/Service/Downloads/downloads_node.html) stehen online zum Download bereit.


## query
Im JSON-Format lassen sich aktuelle und historische Daten zu ausgewählten Indikatoren über GET-requests folgender Machart erhalten:

```
https://www.karto365.de/hosting/rest/services/{table}/MapServer/0/query?f=json&where=1%3D1&outFields=*&returnGeometry=false
```

Dabei ist *{table}* der Name der angefragten Tabelle (z.B. p_apo_f_ZA2022).

Angaben zu allen online vorliegenden Tabellen (vgl. [hier](https://www.karto365.de/portal/sharing/rest/search?q=deutschlandatlas&f=json&num=100&start=1) und [hier](https://www.karto365.de/portal/sharing/rest/search?q=deutschlandatlas&f=json&num=100&start=101)) und den zentralen enthaltenen Daten (sog. "outFields") finden sich in folgender Tabelle.

Weitere Parameter finden sich unter der Tabelle aufgelistet und erläutert.

|title|snippet|url|x|
|---|---|---|---|
|Basemap_light|Basemap_light|https://www.karto365.de/hosting/rest/services/Basemap_light/MapServer||
|erw_mini_HA2023|Anteil der ausschließlich geringfügig entlohnten Beschäftigten am Arbeitsort an allen Erwerbstätigen im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/erw_mini_HA2023/MapServer|erw_mini|
|pendel_b_HA2023|Durchschnittliche Pendeldistanzen aller SV_Beschäftigten am Wohnort 2021 in km|https://www.karto365.de/hosting/rest/services/pendel_b_HA2023/MapServer|pendel|
|p_nelade_r_HA2023|Pkw_Fahrzeit zur nächsten öffentlich zugänglichen Normalladestation für Elektroautos im Jahr 2023 in Minuten|https://www.karto365.de/hosting/rest/services/p_nelade_r_HA2023/MapServer||
|pendel_a_HA2023|Pendlerverflechtungen zwischen Gemeindeverbänden nach Anzahl der Pendler im Jahr 2021|https://www.karto365.de/hosting/rest/services/pendel_a_HA2023/MapServer|Pendler202|
|heiz_wohn_HA2023|Anteil fertiggestellter Wohnungen mit primär erneuerbarer Heizenergie an allen errichteten Wohnungen in neuen Wohngebäuden im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/heiz_wohn_HA2023/MapServer|heiz_wohn|
|teilz_w_HA2023|Weibliche sozialversicherungspflichtig Beschäftigte in Teilzeit am Arbeitsort an den weiblichen sozialversicherungspflichtig Beschäftigten im Jahr 2022 in _%|https://www.karto365.de/hosting/rest/services/teilz_w_HA2023/MapServer|teilz_w|
|p_freibad_HA2022|Pkw_Fahrzeit zum nächsten Freibad oder Naturbad im Jahr 2020 in Minuten|https://www.karto365.de/hosting/rest/services/p_freibad_HA2022/MapServer|p_freibad|
|preis_miet_HA2023|Wiedervermietungsmieten _Angebotsmieten nettokalt_ im Jahr 2022 in € je m²|https://www.karto365.de/hosting/rest/services/preis_miet_HA2023/MapServer||
|wohn_EFZH_HA2023|Fertiggestellte Wohnungen in neuen Ein_ und Zweifamilienhäusern je 10_000 Einwohner__innen im Jahr 2021|https://www.karto365.de/hosting/rest/services/wohn_EFZH_HA2023/MapServer|wohn_EZFH|
|bev_ausl_HA2023|Anteil der Ausländer__innen an der Gesamtbevölkerung im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/bev_ausl_HA2023/MapServer|bev_ausl|
|bev_u18_HA2023|Anteil der unter 18_Jährigen an der Gesamtbevölkerung im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/bev_u18_HA2023/MapServer|bev_u18|
|schule_oabschl_HA2023|Anteil der Schulabgänger__innen ohne Hauptschulabschluss an allen Schulabgänger__innen allgemeinbildender Schulen im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/schule_oabschl_HA2023/MapServer|schule_oabschl|
|oenv_HA2023|Anteil der Bevölkerung_ die in maximal 600 m bzw_ bei Bahnhöfen 1_200 m Luftlinienentfernung um eine Haltestelle mit mindestens 20 Abfahrten im ÖV am Tag wohnt_ im Jahr 2022 in _%|https://www.karto365.de/hosting/rest/services/oenv_HA2023/MapServer|oenv|
|erw_minineben_HA2023|Anteil der geringfügig entlohnten Beschäftigten im Nebenjob am Arbeitsort an allen Erwerbstätigen im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/erw_minineben_HA2023/MapServer|erw_minineben|
|teilz_m_HA2022|Männliche sozialversicherungspflichtig Beschäftigte in Teilzeit am Arbeitsort an den männlichen sozialversicherungspflichtig Beschäftigten im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/teilz_m_HA2022/MapServer|teilz_m|
|beschq_m_HA2023|Sozialversicherungspflichtig beschäftigte Männer am Wohnort je 100 Männer im erwerbsfähigen Alter im Jahr 2022|https://www.karto365.de/hosting/rest/services/beschq_m_HA2023/MapServer|beschq_m|
|p_kh_gru_b|Pkw_Fahrzeit zum nächsten Krankenhaus mit Grundversorgung im Jahr 2016 in Minuten, K33, p_kh_gru_b, feature|https://www.karto365.de/hosting/rest/services/p_kh_gru_b/MapServer||
|st_einnkr_HA2021|Steuereinnahmekraft je Einwohner__in im Jahr 2018 in €; st_einnkr_HA2021|https://www.karto365.de/hosting/rest/services/st_einnkr_HA2021/MapServer|st_einnkr|
|fl_suv_HA2022|Anteil der Siedlungs_ und Verkehrsfläche an der Gesamtfläche im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/fl_suv_HA2022/MapServer|fl_suv|
|kbetr_u3_ZA2022|Anteil der betreuten Kinder unter 3 Jahren in Kindertageseinrichtungen__tagespflege an der Altersgruppe im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/kbetr_u3_ZA2022/MapServer|kbetr_u3|
|p_elade_HA2022|Pkw_Fahrzeit zur nächsten Ladestation für Elektroautos im Jahr 2020 in Minuten|https://www.karto365.de/hosting/rest/services/p_elade_HA2022/MapServer|p_elade|
|fl_suv_ZA2023|Anteil der Siedlungs_ und Verkehrsfläche an der Gesamtfläche im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/fl_suv_ZA2023/MapServer|fl_suv|
|ko_kasskred_HA2022|Kommunale Kassenkredite je Einwohner__in im Jahr 2020 in €|https://www.karto365.de/hosting/rest/services/ko_kasskred_HA2022/MapServer|ko_kasskred|
|alq_HA2023|Arbeitslosenquote bezogen auf alle zivilen Erwerbspersonen im Jahr 2022 in _%|https://www.karto365.de/hosting/rest/services/alq_HA2023/MapServer|alq|
|p_markt_b|p_markt_b, feature|https://www.karto365.de/hosting/rest/services/p_markt_b/MapServer||
|v_breitb1000_HA2023|Anteil der Haushalte_ die mit einer Internetgeschwindigkeit von ≥ 1_000 Mbit_s versorgt werden können_ im Juni 2022 in _%|https://www.karto365.de/hosting/rest/services/v_breitb1000_HA2023/MapServer|v_breitb1000|
|erw_vol_HA2023|Veränderung des Arbeitsvolumens am Arbeitsort 2014 zu 2020 in _%|https://www.karto365.de/hosting/rest/services/erw_vol_HA2023/MapServer|erw_vol|
|v_harzt_HA2023|Hausärzte__ärztinnen je 100_000 Einwohner__innen im Jahr 2020|https://www.karto365.de/hosting/rest/services/v_harzt_HA2023/MapServer|v_harzt|
|fl_landw_HA2022|Anteil der Landwirtschaftsfläche an der Gesamtfläche im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/fl_landw_HA2022/MapServer|fl_landw|
|pfl_stat_wms|Anteil der Pflegebedürftigen in stationärer Pflege im Jahr 2019 an den Pflegebedürftigen insgesamt in _|https://www.karto365.de/hosting/rest/services/pfl_stat_wms/MapServer|pfl_stat|
|bev_ausw_HA2022|Saldo der Außenwanderungen pro 10_000 Einwohner__innen im Jahr 2020|https://www.karto365.de/hosting/rest/services/bev_ausw_HA2022/MapServer|bev_ausw|
|kinder_bg_HA2022|Anteil der unter 15_Jährigen in SGB_II_Bedarfsgemeinschaften an der Altersgruppe im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/kinder_bg_HA2022/MapServer|kinder_bg|
|teilz_w_HA2022|Weibliche sozialversicherungspflichtig Beschäftigte in Teilzeit am Arbeitsort an den weiblichen sozialversicherungspflichtig Beschäftigten im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/teilz_w_HA2022/MapServer|teilz_w|
|VG250_Verbandsgemeinden1219_Punkt|VG250_Verbandsgemeinden1219_Punkt, |https://www.karto365.de/hosting/rest/services/VG250_Verbandsgemeinden1219_Punkt/MapServer||
|bquali_oabschl_HA2022|Anteil sozialversicherungspflichtig Beschäftigter am Arbeitsort ohne einen Berufs__ akademischen Abschluss an allen sozialversicherungspflichtig Beschäftigten im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/bquali_oabschl_HA2022/MapServer|bquali_oabschl|
|elterng_v_HA2022|Anteil der Kinder_ deren Vater Elterngeld bezogen hat_ an allen anspruchsbegründeten Kindern im Jahr 2018 in _|https://www.karto365.de/hosting/rest/services/elterng_v_HA2022/MapServer|elterng_v|
|v_lte_ZA2022|Mobile Breitbandverfügbarkeit mit LTE ab 2 Mbit_s in _ der Fläche im Jahr 2021|https://www.karto365.de/hosting/rest/services/v_lte_ZA2022/MapServer|v_lte|
|kbetr_u3_HA2023|Anteil der betreuten Kinder unter 3 Jahren in Kindertageseinrichtungen__tagespflege an der Altersgruppe im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/kbetr_u3_HA2023/MapServer|kbetr_u3|
|pendel_a_HA2021|Durchschnittliche Pendeldistanzen aller SV_Beschäftigten am Wohnort 2019 in km, pendel_a_HA2021|https://www.karto365.de/hosting/rest/services/pendel_a_HA2021/MapServer|pendel|
|p_hbad_HA2022|Pkw_Fahrzeit zum nächsten Hallenbad im Jahr 2020 in Minuten|https://www.karto365.de/hosting/rest/services/p_hbad_HA2022/MapServer|p_hbad|
|p_nelade_f_HA2023|Mittlere Pkw_Fahrzeit zur nächsten öffentlich zugänglichen Normalladestation für Elektroautos im Jahr 2023|https://www.karto365.de/hosting/rest/services/p_nelade_f_HA2023/MapServer||
|VG250_Gemeinden1220_Punkt|VG250_Gemeinden1220_Punkt, feature to point, dann nur punktlayer beschriftet|https://www.karto365.de/hosting/rest/services/VG250_Gemeinden1220_Punkt/MapServer||
|erw_vol_HA2022|Veränderung des Arbeitsvolumens am Arbeitsort 2014 zu 2019 in _|https://www.karto365.de/hosting/rest/services/erw_vol_HA2022/MapServer|erw_vol|
|ko_kasskred_HA2023|Kommunale Kassenkredite je Einwohner__in im Jahr 2021 in €|https://www.karto365.de/hosting/rest/services/ko_kasskred_HA2023/MapServer|ko_kasskred|
|sozsich_ZA2023|Anteil der Personen in sozialer Mindestsicherung an allen Einwohnerinnen und Einwohnern im Jahr 2020 in _%|https://www.karto365.de/hosting/rest/services/sozsich_ZA2023/MapServer|sozsich|
|teilz_insg_HA2022|Anteil der sozialversicherungspflichtig Beschäftigten in Teilzeit am Arbeitsort an den sozialversicherungspflichtig Beschäftigten im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/teilz_insg_HA2022/MapServer|teilz_insg|
|p_selade_r_HA2023|Pkw_Fahrzeit zur nächsten öffentlich zugänglichen Schnellladestation für Elektroautos im Jahr 2023 in Minuten|https://www.karto365.de/hosting/rest/services/p_selade_r_HA2023/MapServer||
|VG250_Kreise1219_Punkt| tahoma 10 schwarz, zuerst features in punkte; Beste Platzierung 214|https://www.karto365.de/hosting/rest/services/VG250_Kreise1219_Punkt/MapServer||
|v_breitb50_HA2021|Anteil der Haushalte, die mit einer Internetgeschwindigkeit von mindestens 1000 Mbit/s versorgt werden können im Jahr 2020 in %|https://www.karto365.de/hosting/rest/services/v_breitb50_HA2021/MapServer|v_breitb50|
|ko_kasskred_HA2021|Kommunale Kassenkredite je Einwohner__in im Jahr 2019 in €, ko_kasskred_HA2021|https://www.karto365.de/hosting/rest/services/ko_kasskred_HA2021/MapServer|ko_kasskred|
|schulden_HA2023|Anteil überschuldeter Personen über 18 Jahre an der Altersgruppe im Jahr 2022 in _%|https://www.karto365.de/hosting/rest/services/schulden_HA2023/MapServer|schulden|
|p_kh_sm_b|p_kh_sm_b, feature|https://www.karto365.de/hosting/rest/services/p_kh_sm_b/MapServer||
|alq_HA2022_2|Arbeitslosenquote bezogen auf alle zivilen Erwerbspersonen im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/alq_HA2022_2/MapServer|alq|
|wohn_EZFH_ZA2022|Fertiggestellte Wohnungen in neuen Ein_ und Zweifamilienhäusern je 10_000 Einwohner__innen im Jahr 2020|https://www.karto365.de/hosting/rest/services/wohn_EZFH_ZA2022/MapServer|wohn_EZFH|
|wohn_leer_HA2021|Anteil leer stehender Wohnungen an allen Wohnungen 2018 in %, wohn_leer_HA2021|https://www.karto365.de/hosting/rest/services/wohn_leer_HA2021/MapServer||
|kbetr_ue6_ZA2022|Anteil der betreuten Kinder ab 6 bis unter 11 Jahren in Kindertageseinrichtungen__tagespflege an der Altersgruppe im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/kbetr_ue6_ZA2022/MapServer|kbetr_ue6|
|kbetr_ue3_ZA2022|Anteil der betreuten Kinder ab 3 bis unter 6 Jahren in Kindertageseinrichtungen__tagespflege an der Altersgruppe im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/kbetr_ue3_ZA2022/MapServer|kbetr_ue3|
|elade_HA2022|Öffentlich zugängliche Ladepunkte für Elektrofahrzeuge im Jahr 2021 je 100_000 Einwohner__innen|https://www.karto365.de/hosting/rest/services/elade_HA2022/MapServer|elade|
|fl_wald_HA2022|Anteil der Waldfläche an der Gesamtfläche im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/fl_wald_HA2022/MapServer|fl_wald|
|teilz_w_HA2021|Weibliche sozialversicherungspflichtig Beschäftigte in Teilzeit am Arbeitsort je 100 weibliche Einwohner im erwerbsfähigen Alter im Jahr 2020, teilz_w_HA2021|https://www.karto365.de/hosting/rest/services/teilz_w_HA2021/MapServer|teilz_w|
|v_lte_wms|Mobile Breitbandverfügbarkeit mit LTE ab 2 Mbit_s in _ der Fläche im Jahr 2021|https://www.karto365.de/hosting/rest/services/v_lte_wms/MapServer|v_lte|
|bev_18_65_HA2023|Anteil der 18_ bis unter 65_Jährigen an der Gesamtbevölkerung im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/bev_18_65_HA2023/MapServer|bev_18_65|
|bev_ausl_HA2021|Anteil der Ausländer__innen an der Gesamtbevölkerung im Jahr 2019 in %, bev_ausl_HA2021|https://www.karto365.de/hosting/rest/services/bev_ausl_HA2021/MapServer|bev_ausl|
|v_breitb50_HA2023|Anteil der Haushalte_ die mit einer Internetgeschwindigkeit von _ 50 Mbit_s versorgt werden können_ im Juni 2022 in _%|https://www.karto365.de/hosting/rest/services/v_breitb50_HA2023/MapServer|v_breitb50|
|erw_mini_ZA2022|Anteil der ausschließlich geringfügig entlohnten Beschäftigten am Arbeitsort an allen Erwerbstätigen im Jahr 2019 in _|https://www.karto365.de/hosting/rest/services/erw_mini_ZA2022/MapServer|erw_mini|
|kinder_bg_wms|Anteil der unter 15_Jährigen in SGB_II_Bedarfsgemeinschaften an der Altersgruppe im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/kinder_bg_wms/MapServer|kinder_bg|
|beschq_insg_HA2022|Sozialversicherungspflichtig Beschäftigte am Wohnort je 100 Einwohner__innen im erwerbsfähigen Alter im Jahr 2021|https://www.karto365.de/hosting/rest/services/beschq_insg_HA2022/MapServer|beschq_insg|
|preis_miet_HA2022|Wiedervermietungsmieten _Angebotsmieten nettokalt_ im Jahr 2021 in € je m²|https://www.karto365.de/hosting/rest/services/preis_miet_HA2022/MapServer||
|wahl_beteil_wms|Bundestagswahlbeteiligung 2021 in Kreisen in _|https://www.karto365.de/hosting/rest/services/wahl_beteil_wms/MapServer|wahl_beteil|
|bev_ue65_HA2021|Anteil der 65_Jährigen und Älteren an der Gesamtbevölkerung im Jahr 2019 in %, bev_ue65_HA2021|https://www.karto365.de/hosting/rest/services/bev_ue65_HA2021/MapServer|bev_ue65|
|beschq_m_HA2022|Sozialversicherungspflichtig beschäftigte Männer am Wohnort je 100 Männer im erwerbsfähigen Alter im Jahr 2021|https://www.karto365.de/hosting/rest/services/beschq_m_HA2022/MapServer|beschq_m|
|st_einnkr_ZA2023|Steuereinnahmekraft je Einwohner__in im Jahr 2021 in €|https://www.karto365.de/hosting/rest/services/st_einnkr_ZA2023/MapServer|st_einnkr|
|luftrtng_b|luftrtng, k36, feature|https://www.karto365.de/hosting/rest/services/luftrtng_b/MapServer||
|einbr_HA2022|Fälle von Wohnungseinbruchdiebstahl pro 100_000 Einwohner__innen im Jahr 2021|https://www.karto365.de/hosting/rest/services/einbr_HA2022/MapServer|einbr|
|p_sek_1_a|Pkw_Fahrzeit zur nächsten Schule der Sekundarstufe I im Jahr 2015_16_17 in Minuten, K41, p_sek_1|https://www.karto365.de/hosting/rest/services/p_sek_1_a/MapServer||
|erw_wachs_HA2023|Gemittelte Entwicklung der Erwerbstätigenzahl am Arbeitsort von 2011 bis 2021 pro Jahr in _%|https://www.karto365.de/hosting/rest/services/erw_wachs_HA2023/MapServer|erw_wachs|
|bev_ue65_HA2023|Anteil der 65_Jährigen und Älteren an der Gesamtbevölkerung im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/bev_ue65_HA2023/MapServer|bev_ue65|
|p_apo_f_ZA2022|Pkw_Fahrzeit zum nächsten öffentlichen Apotheke im Jahr 2020 in Minuten|https://www.karto365.de/hosting/rest/services/p_apo_f_ZA2022/MapServer||
|bev_entw_ZA2022|Gemittelte Entwicklung der Bevölkerungszahl zwischen 2015 und 2020 pro Jahr in _|https://www.karto365.de/hosting/rest/services/bev_entw_ZA2022/MapServer|bev_entw|
|wohn_MFH_ZA2022|Fertiggestellte Wohnungen in neuen Mehrfamilienhäusern je 10_000 Einwohner__innen im Jahr 2020|https://www.karto365.de/hosting/rest/services/wohn_MFH_ZA2022/MapServer|wohn_MFH|
|eauto_HA2022|Anteil von Pkw mit reinem Elektroantrieb _BEV_ an allen Pkw im Jahr 2022 in _|https://www.karto365.de/hosting/rest/services/eauto_HA2022/MapServer|eauto|
|kinder_bg_HA2021|Anteil der unter 15_Jährigen in SGB_II_Bedarfsgemeinschaften an der Altersgruppe im Jahr 2019 in %, kinder_bg_HA2021|https://www.karto365.de/hosting/rest/services/kinder_bg_HA2021/MapServer|kinder_bg|
|bev_u18_HA2021|Anteil der unter 18_Jährigen an der Gesamtbevölkerung im Jahr 2019 in %, , bev_u18_HA2021|https://www.karto365.de/hosting/rest/services/bev_u18_HA2021/MapServer|bev_u18|
|schule_oabschl_HA2022|Anteil der Schulabgänger__innen ohne Hauptschulabschluss an allen Schulabgänger__innen allgemeinbildender Schulen im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/schule_oabschl_HA2022/MapServer|schule_oabschl|
|beschq_insg_HA2021|Sozialversicherungspflichtig Beschäftigte am Wohnort je 100 Einwohner__innen im erwerbsfähigen Alter im Jahr 2020; beschq_insg_HA2021|https://www.karto365.de/hosting/rest/services/beschq_insg_HA2021/MapServer|beschq_insg|
|v_harzt_HA2021|Hausärzte__ärztinnen im Jahr 2017 je 100_000 Einwohner__innen|https://www.karto365.de/hosting/rest/services/v_harzt_HA2021/MapServer|v_harzt|
|bev_ue65_ZA2022|Anteil der 65_Jährigen und Älteren an der Gesamtbevölkerung im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/bev_ue65_ZA2022/MapServer|bev_ue65|
|p_hbad_f_HA2022|feautre abfrage für p_hbad|https://www.karto365.de/hosting/rest/services/p_hbad_f_HA2022/MapServer||
|VG250_GEM1217_neu|VG250_GEM1217_neu|https://www.karto365.de/hosting/rest/services/VG250_GEM1217_neu/MapServer||
|kbetr_ue3_HA2023|Anteil der betreuten Kinder ab 3 bis unter 6 Jahren in Kindertageseinrichtungen_ _tagespflege an der Altersgruppe im Jahr 2021 in _%|https://www.karto365.de/hosting/rest/services/kbetr_ue3_HA2023/MapServer|kbetr_ue3|
|erw_mini_ZA2023|Anteil der ausschließlich geringfügig entlohnten Beschäftigten am Arbeitsort an allen Erwerbstätigen im Jahr 2020 in _%|https://www.karto365.de/hosting/rest/services/erw_mini_ZA2023/MapServer|erw_mini|
|grusi_ZA2022|Anteil der Bevölkerung mit Grundsicherung im Alter an den 65_Jährigen und Älteren im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/grusi_ZA2022/MapServer|grusi|
|wohn_MFH_HA2023|Fertiggestellte Wohnungen in neuen Mehrfamilienhäusern je 10_000 Einwohner__innen im Jahr 2021|https://www.karto365.de/hosting/rest/services/wohn_MFH_HA2023/MapServer|wohn_MFH|
|grusi_wms|Anteil der Bevölkerung mit Grundsicherung im Alter an den 65_Jährigen und Älteren im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/grusi_wms/MapServer|grusi|
|kbtr_pers_HA2021|Plätze in Kindertageseinrichtungen je pädagogisch tätige Person im Jahr 2019, kbtr_pers_HA2021|https://www.karto365.de/hosting/rest/services/kbtr_pers_HA2021/MapServer|kbtr_pers|
|VG250_Verbandsgemeinden_1220_Punkt|VG250_Verbandsgemeinden_1220_Punkt, feature to point, dann punktelaer beschriftet|https://www.karto365.de/hosting/rest/services/VG250_Verbandsgemeinden_1220_Punkt/MapServer||
|wohn_EZFH_HA2021|Fertiggestellte Wohnungen in neuen Ein_ und Zweifamilienhäusern je 10_000 Einwohner__innen im Jahr 2019, wohn_EZFH_HA2021|https://www.karto365.de/hosting/rest/services/wohn_EZFH_HA2021/MapServer|wohn_EZFH|
|bev_binw_HA2022|Saldo der Binnenwanderungen pro 10_000 Einwohner__innen im Jahr 2020|https://www.karto365.de/hosting/rest/services/bev_binw_HA2022/MapServer|bev_binw|
|p_ozmz_oev_r_HA2021|Reisezeit mit dem Öffentlichen Verkehr _ÖV_ zum Stadtzentrum des nächsten Ober_ oder Mittelzentrum 2020 in Minuten, p_ozmz_oev_r_HA2021, Raster|https://www.karto365.de/hosting/rest/services/p_ozmz_oev_r_HA2021/MapServer||
|bquali_unifh_HA2022|Anteil sozialversicherungspflichtig Beschäftigter am Arbeitsort mit einem akademischen Abschluss an allen sozialversicherungspflichtig Beschäftigten im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/bquali_unifh_HA2022/MapServer|bquali_unifh|
|schulden_HA2022|Anteil überschuldeter Personen über 18 Jahre an der Altersgruppe im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/schulden_HA2022/MapServer|schulden|
|fl_landw_HA2021|Anteil der Landwirtschaftsfläche an der Gesamtfläche im Jahr 2019 in %, fl_landw_HA2021|https://www.karto365.de/hosting/rest/services/fl_landw_HA2021/MapServer|fl_landw|
|p_selade_f_HA2023|Mittlere Pkw_Fahrzeit zur nächsten öffentlich zugänglichen Schnellladestation für Elektroautos im Jahr 2023|https://www.karto365.de/hosting/rest/services/p_selade_f_HA2023/MapServer||
|grusi_HA2023|Anteil der Bevölkerung mit Grundsicherung im Alter an den 65_Jährigen und Älteren im Jahr 2022 in _%|https://www.karto365.de/hosting/rest/services/grusi_HA2023/MapServer|grusi|
|VG250_Kreise_1221_Punkte|VG250_Kreise_1221_Punkte, Feature to Point, dann Punktelayer beschriftet|https://www.karto365.de/hosting/rest/services/VG250_Kreise_1221_Punkte/MapServer||
|kbtr_pers_wms|Plätze in Kindertageseinrichtungen je pädagogisch tätige Person im Jahr 2021|https://www.karto365.de/hosting/rest/services/kbtr_pers_wms/MapServer|kbtr_pers|
|beschq_w_HA2022|Sozialversicherungspflichtig beschäftigte Frauen am Wohnort je 100 Frauen im erwerbsfähigen Alter im Jahr 2021|https://www.karto365.de/hosting/rest/services/beschq_w_HA2022/MapServer|beschq_w|
|erw_bip_HA2021|Bruttoinlandsprodukt je erwerbstätige Person im Jahr 2018 in 1_000 €, erw_bip_HA2021|https://www.karto365.de/hosting/rest/services/erw_bip_HA2021/MapServer|erw_bip|
|hh_veink_ZA2022|Verfügbares Einkommen privater Haushalte je Einwohner__in im Jahr 2019 in 1_000 €|https://www.karto365.de/hosting/rest/services/hh_veink_ZA2022/MapServer|hh_veink|
|bev_entw_HA2023|Gemittelte Entwicklung der Bevölkerungszahl zwischen 2016 und 2021 pro Jahr in _%|https://www.karto365.de/hosting/rest/services/bev_entw_HA2023/MapServer|bev_entw|
|beschq_w_HA2023|Sozialversicherungspflichtig beschäftigte Frauen am Wohnort je 100 Frauen im erwerbsfähigen Alter im Jahr 2022|https://www.karto365.de/hosting/rest/services/beschq_w_HA2023/MapServer|beschq_w|
|p_elade_f_HA2022|feature abfrage layer für p_elade|https://www.karto365.de/hosting/rest/services/p_elade_f_HA2022/MapServer||
|bev_dicht_HA2023|Einwohner__innen je km² im Jahr 2021|https://www.karto365.de/hosting/rest/services/bev_dicht_HA2023/MapServer|bev_dicht|
|p_ozmz_miv_f_HA2021|p_ozmz_miv_f_HA2021, Feature|https://www.karto365.de/hosting/rest/services/p_ozmz_miv_f_HA2021/MapServer||
|pfl_ambu_ZA2022|Anteil der Pflegebedürftigen in ambulanter Pflege an den Pflegebedürftigen insgesamt im Jahr 2019 in _|https://www.karto365.de/hosting/rest/services/pfl_ambu_ZA2022/MapServer|pfl_ambu|
|wohn_MFH_HA2021|Fertiggestellte Wohnungen in neuen Mehrfamilienhäusern je 10_000 Einwohner__innen im Jahr 2019, wohn_MFH_HA2021|https://www.karto365.de/hosting/rest/services/wohn_MFH_HA2021/MapServer|wohn_MFH|
|bev_entw_ZA2021|Gemittelte Entwicklung der Bevölkerungszahl zwischen 2014 und 2019 pro Jahr in %, k3, bev_entw_ZA2021|https://www.karto365.de/hosting/rest/services/bev_entw_ZA2021/MapServer|bev_entw|
|p_hbad_r_HA2022|Pkw_Fahrzeit zum nächsten Hallenband im Jahr 2020 in Minuten|https://www.karto365.de/hosting/rest/services/p_hbad_r_HA2022/MapServer||
|wohn_EZFH_HA2023|Fertiggestellte Wohnungen in neuen Ein_ und Zweifamilienhäusern je 10_000 Einwohner__innen im Jahr 2021|https://www.karto365.de/hosting/rest/services/wohn_EZFH_HA2023/MapServer|wohn_EZFH|
|fl_suv_HA2021|Anteil der Siedlungs_ und Verkehrsfläche an der Gesamtfläche im Jahr 2019 in %, fl_suv_HA2021|https://www.karto365.de/hosting/rest/services/fl_suv_HA2021/MapServer|fl_suv|
|bquali_unifh_HA2021|Anteil sozialversicherungspflichtig Beschäftigter am Arbeitsort mit einem akademischen Abschluss an allen sozialversicherungspflichtig Beschäftigten im Jahr 2020 in %, bquali_unifh_HA2021|https://www.karto365.de/hosting/rest/services/bquali_unifh_HA2021/MapServer|bquali_unifh|
|luftrtng_a|Erreichbarkeit durch Luftrettung während des Tages im Jahr 2016 in Minuten, luftrtng, K36, Raster|https://www.karto365.de/hosting/rest/services/luftrtng_a/MapServer||
|p_grunds_b|p_grunds_b, feature|https://www.karto365.de/hosting/rest/services/p_grunds_b/MapServer||
|p_ozmz_miv_r_HA2021|Pkw_Fahrzeit zum Stadtzentrum des nächsten Ober_ oder Mittelzentrum 2020 in Minuten, p_ozmz_miv_r_HA2021, Raster|https://www.karto365.de/hosting/rest/services/p_ozmz_miv_r_HA2021/MapServer||
|preis_miet_HA2021|Wiedervermietungsmieten in mittlerer_guter Wohnlage _Angebotsmieten nettokalt_ 2020 in € je m², preis_miet_HA2021|https://www.karto365.de/hosting/rest/services/preis_miet_HA2021/MapServer||
|p_poli_a|Pkw_Fahrzeit von der nächsten Polizeidienststelle im Jahr 2014 in Minuten, K50, p_poli_a|https://www.karto365.de/hosting/rest/services/p_poli_a/MapServer||
|straft_HA2021|Straftaten insgesamt pro 100_000 Einwohner__innen im Jahr 2020, straft_HA2021|https://www.karto365.de/hosting/rest/services/straft_HA2021/MapServer|straft|
|bev_entw_wms|Gemittelte Entwicklung der Bevölkerungszahl zwischen 2015 und 2020 pro Jahr in _|https://www.karto365.de/hosting/rest/services/bev_entw_wms/MapServer|bev_entw|
|v_breitb50_HA2022|Anteil der Haushalte_ die mit einer Internetgeschwindigkeit von mindestens 50 Mbit_s versorgt werden können_ im Juni 2021 in _|https://www.karto365.de/hosting/rest/services/v_breitb50_HA2022/MapServer|v_breitb50|
|erw_minineben_ZA2023|Anteil der geringfügig entlohnten Beschäftigten im Nebenjob am Arbeitsort an allen Erwerbstätigen im Jahr 2020 in _&|https://www.karto365.de/hosting/rest/services/erw_minineben_ZA2023/MapServer|erw_minineben|
|alq_HA2022|Arbeitslosenquote bezogen auf alle zivilen Erwerbspersonen im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/alq_HA2022/MapServer|alq|
|p_harzt_b|K31, p_harzt_b, featureinfo|https://www.karto365.de/hosting/rest/services/p_harzt_b/MapServer||
|heiz_wohn_HA2022|Anteil fertiggestellter Wohnungen mit primär erneuerbarer Heizenergie an allen errichteten Wohnungen in neuen Wohngebäuden im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/heiz_wohn_HA2022/MapServer|heiz_wohn|
|VG250_v_lte_Grenzen|VG250_v_lte_Grenzen|https://www.karto365.de/hosting/rest/services/VG250_v_lte_Grenzen/MapServer||
|fl_wald_HA2021|Anteil der Waldfläche an der Gesamtfläche im Jahr 2019 in %, fl_wald_HA2021|https://www.karto365.de/hosting/rest/services/fl_wald_HA2021/MapServer|fl_wald|
|erw_vol_HA2021|Anteil der Pflegebedürftigen in ambulanter Pflege im Jahr 2017 an den Pflegebedürftigen insgesamt in _|https://www.karto365.de/hosting/rest/services/erw_vol_HA2021/MapServer|erw_vol|
|p_ozmz_b|Durchschnittliche bevölkerungsgewichtete Pkw-Fahrzeit zum Stadtzentrum des nächst_en Ober- oder Mittelzentrum 2019 in Minuten, K29, p_ozmz|https://www.karto365.de/hosting/rest/services/p_ozmz_b/MapServer||
|kbetr_ue3_HA2021|Anteil der betreuten Kinder zwischen 3 und 6 Jahren in Kindertageseinrichtungen__tagespflege an der Altersgruppe im Jahr 2019 in _, kbetr_ue3_HA2021|https://www.karto365.de/hosting/rest/services/kbetr_ue3_HA2021/MapServer|kbetr_ue3|
|schule_oabschl_HA2021|Anteil der Schulabgänger__innen ohne Hauptschulabschluss an allen Schulabgänger__innen allgemeinbildender Schulen im Jahr 2019 in %, schule_oabschl_HA2021|https://www.karto365.de/hosting/rest/services/schule_oabschl_HA2021/MapServer|schule_oabschl|
|pfl_geld_ZA2022|Anteil der Pflegegeldempfänger__innen im Jahr 2019 an den Pflegebedürftigen insgesamt in _|https://www.karto365.de/hosting/rest/services/pfl_geld_ZA2022/MapServer|pfl_geld|
|erw_bip_ZA2023|Bruttoinlandsprodukt je erwerbstätige Person im Jahr 2020 in 1_000 €|https://www.karto365.de/hosting/rest/services/erw_bip_ZA2023/MapServer|erw_bip|
|p_apo_b|p_apo, feature|https://www.karto365.de/hosting/rest/services/p_apo_b/MapServer||
|p_ozmz_oev_f_HA2021|p_ozmz_oev_f_HA2021, feature|https://www.karto365.de/hosting/rest/services/p_ozmz_oev_f_HA2021/MapServer||
|kbetr_ue6_HA2021|Anteil der betreuten Kinder ab 6 bis unter 11 Jahren in Kindertageseinrichtungen__tagespflege an der Altersgruppe im Jahr 2019 in %, kbetr_ue6_HA2021|https://www.karto365.de/hosting/rest/services/kbetr_ue6_HA2021/MapServer|kbetr_ue6|
|teilz_m_HA2021|Männliche sozialversicherungspflichtig Beschäftigte in Teilzeit am Arbeitsort je 100 männliche Einwohner im erwerbsfähigen Alter im Jahr 2020, teilz_m_HA2021|https://www.karto365.de/hosting/rest/services/teilz_m_HA2021/MapServer|teilz_m|
|erw_wachs_ZA2023|Gemittelte Entwicklung der Erwerbstätigenzahl am Arbeitsort von 2010 bis 2020 pro Jahr in _|https://www.karto365.de/hosting/rest/services/erw_wachs_ZA2023/MapServer|erw_wachs|
|p_apo_a|Pkw_Fahrzeit zum nächsten öffentlichen Apotheke im Jahr 2013 in Minuten, K35, p_apo_a|https://www.karto365.de/hosting/rest/services/p_apo_a/MapServer||
|sozsich_HA2021|Anteil der Personen in sozialer Mindestsicherung an allen Einwohnerinnen und Einwohnern im Jahr 2019 in %, sozsich_HA2021|https://www.karto365.de/hosting/rest/services/sozsich_HA2021/MapServer|sozsich|
|v_harzt_HA2022|Hausärzte__ärztinnen je 100_000 Einwohner__innen im Jahr 2019|https://www.karto365.de/hosting/rest/services/v_harzt_HA2022/MapServer|v_harzt|
|oenv_wms|Anteil der Bevölkerung_ die in maximal 600 m bzw_ bei Bahnhöfen 1_200 m Luftlinienentfernung um eine Haltestelle mit mindestens 20 Abfahrten im ÖV am Tag wohnt_ im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/oenv_wms/MapServer|oenv|
|wahl_beteil_HA2022|Bundestagswahlbeteiligung 2021 in Kreisen in _|https://www.karto365.de/hosting/rest/services/wahl_beteil_HA2022/MapServer|wahl_beteil|
|grusi_ZA2023|Anteil der Bevölkerung mit Grundsicherung im Alter an den 65_Jährigen und Älteren im Jahr 2021 in _|https://www.karto365.de/hosting/rest/services/grusi_ZA2023/MapServer|grusi|
|p_harzt_a|Pkw_Fahrzeit zur nächsten Hausärztin oder zum nächsten Hausarzt im Jahr 2016 in Minuten, K31, p_harzt_a|https://www.karto365.de/hosting/rest/services/p_harzt_a/MapServer||
|kbtr_pers_ZA2022|Plätze in Kindertageseinrichtungen je pädagogisch tätige Person im Jahr 2021|https://www.karto365.de/hosting/rest/services/kbtr_pers_ZA2022/MapServer|kbtr_pers|
|schulden_HA2021|Anteil überschuldeter Personen über 18 Jahren an der Altersgruppe im Jahr 2020 in %, HA2021|https://www.karto365.de/hosting/rest/services/schulden_HA2021/MapServer|schulden|
|elterng_v_HA2021|Anteil der Kinder_ für die mindestens ein männlicher Leistungsbezieher Elterngeld erhalten hat_ an allen anspruchsbegründenden Kindern im Jahr 2017 in %, elterng_v_HA2021|https://www.karto365.de/hosting/rest/services/elterng_v_HA2021/MapServer|elterng_v|
|p_markt_a|Pkw_Fahrzeit zum nächsten Supermarkt oder Discounter im Jahr 2017 in Minuten, K30, p_markt|https://www.karto365.de/hosting/rest/services/p_markt_a/MapServer||
|wahl_beteil|Bundestagswahlbeteiligung 2017 in Gemeinden in %, K10, wahl_beteil|https://www.karto365.de/hosting/rest/services/wahl_beteil/MapServer|wahl_beteil|
|bev_binw_HA2021|Saldo der Binnenwanderungen pro 10_000 Einwohner__innen im Jahr 2019; bev_binw_HA2021|https://www.karto365.de/hosting/rest/services/bev_binw_HA2021/MapServer|bev_binw|
|bev_ausl_ZA2022|Anteil der Ausländer__innen an der Gesamtbevölkerung im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/bev_ausl_ZA2022/MapServer|bev_ausl|
|hh_veink_ZA2023|Verfügbares Einkommen privater Haushalte je Einwohner__in im Jahr 2020 in 1_000 €|https://www.karto365.de/hosting/rest/services/hh_veink_ZA2023/MapServer|hh_veink|
|pfl_ambu_HA2021|Anteil der Pflegebedürftigen in ambulanter Pflege im Jahr 2017 an den Pflegebedürftigen insgesamt in %, pfl_ambu_HA2021|https://www.karto365.de/hosting/rest/services/pfl_ambu_HA2021/MapServer|pfl_ambu|
|erw_minineben_HA2021|Anteil der geringfügig entlohnten Beschäftigten im Nebenjob am Arbeitsort an allen Erwerbstätigen 2018 in %, erw_minineben_HA2021|https://www.karto365.de/hosting/rest/services/erw_minineben_HA2021/MapServer|erw_minineben|
|v_breitb1000_HA2021|Anteil der Haushalte, die mit einer Internetgeschwindigkeit von mindestens 1000 Mbit/s versorgt werden können im Jahr 2020 in %|https://www.karto365.de/hosting/rest/services/v_breitb1000_HA2021/MapServer|v_breitb1000|
|einbr_HA2021|Fälle von Wohnungseinbruchdiebstahl pro 100_000 Einwohner__innen im Jahr 2020, einbr_HA2021|https://www.karto365.de/hosting/rest/services/einbr_HA2021/MapServer|einbr|
|p_kh_gru_a|Pkw_Fahrzeit zum nächsten Krankenhaus mit Grundversorgung im Jahr 2016 in Minuten; K33, p_kh_gru|https://www.karto365.de/hosting/rest/services/p_kh_gru_a/MapServer||
|pfl_stat_ZA2022|Anteil der Pflegebedürftigen in stationärer Pflege an den Pflegebedürftigen insgesamt im Jahr 2019 in _|https://www.karto365.de/hosting/rest/services/pfl_stat_ZA2022/MapServer|pfl_stat|
|teilz_insg_HA2021|Anteil der sozialversicherungspflichtig Beschäftigten in Teilzeit am Arbeitsort an den sozialversicherungspflichtig Beschäftigten im Jahr 2020 in %, teilz_insg_HA2021|https://www.karto365.de/hosting/rest/services/teilz_insg_HA2021/MapServer|teilz_insg|
|erw_mini_HA2021|Anteil der ausschließlich geringfügig entlohnten Beschäftigten am Arbeitsort an allen Erwerbstätigen 2018 in %, erw_mini_HA2021|https://www.karto365.de/hosting/rest/services/erw_mini_HA2021/MapServer|erw_mini|
|beschq_m_HA2021|Sozialversicherungspflichtig beschäftigte Männer am Wohnort je 100 Männer im erwerbsfähigen Alter im Jahr 2020, beschq_m_HA2021|https://www.karto365.de/hosting/rest/services/beschq_m_HA2021/MapServer|beschq_m|
|einbr_wms|Fälle von Wohnungseinbruchdiebstahl pro 100_000 Einwohner__innen im Jahr 2021|https://www.karto365.de/hosting/rest/services/einbr_wms/MapServer|einbr|
|pfl_geld_HA2021|Anteil der Pflegegeldempfänger__innen im Jahr 2017 an den Pflegebedürftigen insgesamt in _, pfl_geld_HA2021|https://www.karto365.de/hosting/rest/services/pfl_geld_HA2021/MapServer|pfl_geld|
|bev_u18_za2022|Anteil der unter 18_Jährigen an der Gesamtbevölkerung im Jahr 2020 in _|https://www.karto365.de/hosting/rest/services/bev_u18_za2022/MapServer|bev_u18|
|erw_minineben_ZA2022|Anteil der geringfügig entlohnten Beschäftigten im Nebenjob am Arbeitsort an allen Erwerbstätigen im Jahr 2019 in _|https://www.karto365.de/hosting/rest/services/erw_minineben_ZA2022/MapServer|erw_minineben|
|oenv_HA2021|Anteil der Bevölkerung_ die in maximal 600 m bzw_ bei Bahnhöfen 1_200 m Luftlinienentfernung um eine Haltestelle mit mindestens 20 Abfahrten im ÖV am Tag wohnt_ im Jahr 2020 in %, oenv_HA2021|https://www.karto365.de/hosting/rest/services/oenv_HA2021/MapServer|oenv|
|p_freibad_r_HA2022|Pkw_Fahrzeit zum nächsten Natur_ oder Freibad im Jahr 2020 in Minuten|https://www.karto365.de/hosting/rest/services/p_freibad_r_HA2022/MapServer||
|p_freibad_f_HA2022|feature abfrage layer für p_freibad|https://www.karto365.de/hosting/rest/services/p_freibad_f_HA2022/MapServer||
|elternv_g_HA2023|Anteil der Kinder_ deren Vater Elterngeld bezogen hat an allen anspruchsbegründeten Kindern im Jahr 2019 in _%|https://www.karto365.de/hosting/rest/services/elternv_g_HA2023/MapServer|elterng_v|
|teilz_m_HA2023|Männliche sozialversicherungspflichtig Beschäftigte in Teilzeit am Arbeitsort an den männlichen sozialversicherungspflichtig Beschäftigten im Jahr 2022 in _%|https://www.karto365.de/hosting/rest/services/teilz_m_HA2023/MapServer|teilz_m|
|p_sek_2_b|p_sek_2_b, feature|https://www.karto365.de/hosting/rest/services/p_sek_2_b/MapServer||
|elade_ZA2023|Öffentlich zugängliche Ladepunkte für Elektrofahrzeuge im Jahr 2022 je 100_000 Einwohner__innen|https://www.karto365.de/hosting/rest/services/elade_ZA2023/MapServer|elade|
|elterng_v_HA2023|Anteil der Kinder_ deren Vater Elterngeld bezogen hat an allen anspruchsbegründeten Kindern im Jahr 2019 in _%|https://www.karto365.de/hosting/rest/services/elterng_v_HA2023/MapServer|elterng_v|
|straft_HA2022|Straftaten insgesamt pro 100_000 Einwohner__innen im Jahr 2021|https://www.karto365.de/hosting/rest/services/straft_HA2022/MapServer|straft|
|bquali_oabschl_HA2021|Anteil sozialversicherungspflichtig Beschäftigter am Arbeitsort ohne einen Berufs__ akademischen Abschluss an allen sozialversicherungspflichtig Beschäftigten im Jahr 2020 in %, bquali_oabschl_HA2021|https://www.karto365.de/hosting/rest/services/bquali_oabschl_HA2021/MapServer|bquali_oabschl|
|p_poli_b|K50, feature info, p_poli_b|https://www.karto365.de/hosting/rest/services/p_poli_b/MapServer||
|p_ozmz_a|Durchschnittliche bevölkerungsgewichtete Pkw_Fahrzeit zum Stadtzentrum des nächsten Ober_ oder Mittelzentrum 2019 in Minuten, K29, p_ozmz, raster|https://www.karto365.de/hosting/rest/services/p_ozmz_a/MapServer||
|kbetr_u3_HA2021|Anteil der betreuten Kinder unter 3 Jahren in Kindertageseinrichtungen__tagespflege an der Altersgruppe im Jahr 2019 in %, kbetr_u3_HA2021|https://www.karto365.de/hosting/rest/services/kbetr_u3_HA2021/MapServer|kbetr_u3|
|p_sek_2_a|Pkw_Fahrzeit zur nächsten Schule der Sekundarstufe II im Jahr 2015_2016_2017 in Minuten, K42, p_sek_2_a|https://www.karto365.de/hosting/rest/services/p_sek_2_a/MapServer||
|v_lte_HA2021|Mobile Breitbandverfügbarkeit mit LTE ab 2Mbit_s in _ der Fläche im Jahr 2020, v_lte_HA2021|https://www.karto365.de/hosting/rest/services/v_lte_HA2021/MapServer|anteil_fla|
|grusi_HA2021|Anteil der Bevölkerung mit Grundsicherung im Alter an den 65_Jährigen und Älteren 2020 in _, grusi_HA2021|https://www.karto365.de/hosting/rest/services/grusi_HA2021/MapServer|grusi|
|v_breitb1000_HA2022|Anteil der Haushalte_ die mit einer Internetgeschwindigkeit von mindestens 1_000 Mbit_s versorgt werden können_ im Juni 2021 in _|https://www.karto365.de/hosting/rest/services/v_breitb1000_HA2022/MapServer|v_breitb1000|
|preis_baul_wms|Baulandpreise für Eigenheime im Jahr 2020 in € je m²|https://www.karto365.de/hosting/rest/services/preis_baul_wms/MapServer||
|p_grunds_a|Pkw_Fahrzeit zur nächsten Grundschule im Jahr 2015_16_17 in Minuten, K40, p_grunds|https://www.karto365.de/hosting/rest/services/p_grunds_a/MapServer||
|erw_wachs_ZA2022|Gemittelte Entwicklung der Erwerbstätigenzahl am Arbeitsort von 2009 bis 2019 pro Jahr in _|https://www.karto365.de/hosting/rest/services/erw_wachs_ZA2022/MapServer|erw_wachs|
|preis_baul_ZA2022|Baulandpreise für Eigenheime im Jahr 2020 in € je m²|https://www.karto365.de/hosting/rest/services/preis_baul_ZA2022/MapServer||
|hh_veink_HA2021|Verfügbares Einkommen privater Haushalte je Einwohner__in im Jahr 2018 in 1_000 €, hh_veink_HA2021|https://www.karto365.de/hosting/rest/services/hh_veink_HA2021/MapServer|hh_veink|
|pendel_b_HA2022|Pendlerverflechtungen zwischen Gemeindeverbänden nach Anzahl der Pendler im Jahr 2020|https://www.karto365.de/hosting/rest/services/pendel_b_HA2022/MapServer|Pendler202|
|alq_HA2021|Arbeitslosenquote bezogen auf alle zivilen Erwerbspersonen im Jahr 2020 in %, alq_HA2021|https://www.karto365.de/hosting/rest/services/alq_HA2021/MapServer|alq|


### Parameter

Die Werte aller Parameter müssen URL-codiert sein wie im Beispiel unten verdeutlicht (also z.B. "where=1%3D1" statt "where=1=1"). Weitere Informationen zu den Parametern finden sich [hier](https://www.karto365.de/hosting/sdk/rest/index.html#/Query_Feature_Service_Layer/02ss0000002r000000/)

**Parameter** *where*
Eine WHERE-Klausel für den query-filter.
z.B. "1=1"


**Parameter** *f*
Das Antwortformat. Standardantwortformat ist html.
z.B. "html", "json", "kmz", "geojson", pbf" (vgl. [hier](https://www.karto365.de/hosting/sdk/rest/index.html#/Output_formats/02ss00000078000000/))


**Parameter** *outFields*
Die Liste der Variablen (fields), die in die zurückgegebene Ergebnismenge aufgenommen werden sollen. Diese Liste ist eine durch Kommas getrennte Liste von Variablennamen. Als Wert dieses Parameters können Sie auch den Platzhalter "*" angeben. In diesem Fall enthalten die Abfrageergebnisse alle Feldwerte.


**Parameter** *returnGeometry*
Bei "true" enthält das Ergebnis die Geometrie, die jedem zurückgegebenen Feature zugeordnet ist. Die Voreinstellung ist true.
z.B. "false"


**Parameter** *geometry*
Die Geometrie, die als räumlicher Filter angewendet werden soll. Die Struktur der Geometrie entspricht der Struktur der JSON-Geometrieobjekte, die von der ArcGIS-REST-API zurückgegeben werden. Zusätzlich zu den JSON-Strukturen können Sie die Geometrie von Envelopes und Punkten mit einer einfachen kommagetrennten Syntax angeben.
z.B.
- geometryType=esriGeometryEnvelope&geometry={xmin: -104, ymin: 35.6, xmax: -94.32, ymax: 41}
- geometryType=esriGeometryEnvelope&geometry=-104,35.6,-94.32,41
- geometryType=esriGeometryPoint&geometry=-104,35.6


**Parameter** *geometryType*
Der vom Geometrieparameter angegebene Geometrietyp. Der Geometrietyp kann ein Envelope, ein Punkt, eine Linie oder ein Polygon sein. Der Standardgeometrietyp ist ein Envelope.
z.B. "esriGeometryEnvelope", "esriGeometryPoint", "esriGeometryMultipoint", "esriGeometryPolyline", "esriGeometryPolygon"


**Parameter** *inSR*
Der Raumbezug (spatial reference) der Eingabegeometrie. Der Raumbezug kann entweder als bekannte ID oder als Raumbezugs-JSON-Objekt angegeben werden. Wenn inSR nicht angegeben ist, wird davon ausgegangen, dass sich die Geometrie im Raumbezug des Layers befindet.


**Parameter** *outSR*
Der Raumbezug (spatial reference) der zurückgegebenen Geometrie. Der Raumbezug kann entweder als bekannte ID oder als Raumbezugs-JSON-Objekt angegeben werden. Wenn outSR nicht angegeben ist, wird die Geometrie im Raumbezug der Karte zurückgegeben.
Bei Verwendung von outSR mit pbf verwendet das pbf-Format die Koordinatenquantisierung für layer-queries. Wenn für einen Abfragevorgang kein Ausgaberaumbezug bereitgestellt wird, leitet der Feature-Service Koordinatenquantisierungsparameter aus dem Raumbezug des Layers ab. Wenn die Genauigkeit des Raumbezugs des Layers für die Verwendung durch die Client-Anwendung nicht ausreicht, sollte sie einen Raumbezug mit angemessener Genauigkeit als Ausgabe-Raumbezug übergeben. Wenn der Quell-Raumbezug des Layers die gewünschte Genauigkeit aufweist und für die Verwendung durch den Client geeignet ist, kann der Client den Raumbezug des Quell-Layers als Ausgabe-Raumbezug verwenden.


**Parameter** *objectIds*
Die abzufragenden Objekt-IDs dieses layer oder dieser Tabelle.


**Parameter** *spatialRel*
Die räumliche Beziehung, die beim Ausführen des Query auf die Eingabegeometrie angewendet werden soll. Zu den unterstützten räumlichen Beziehungen gehören Schnittmenge, Enthält, Envelope-Schnittmenge, Innerhalb usw. Die standardmäßige räumliche Beziehung ist Schnittmenge (esriSpatialRelIntersects).
z.B.
"esriSpatialRelIntersects", "esriSpatialRelContains", "esriSpatialRelCrosses", "esriSpatialRelEnvelopeIntersects", "esriSpatialRelIndexIntersects","esriSpatialRelOverlaps","esriSpatialRelTouches","esriSpatialRelWithin"


**Parameter** *distance*
Der Pufferabstand für die Eingabegeometrien. Die Entfernungseinheit wird durch Einheiten angegeben. Wenn die Entfernung beispielsweise 100 beträgt, ist die Abfragegeometrie ein Punkt, die Einheiten werden auf Meter festgelegt, und alle Punkte innerhalb von 100 Metern um den Punkt werden zurückgegeben. Der geodätische Puffer wird basierend auf dem Datum des ausgegebenen Raumbezugs erstellt, sofern vorhanden. Wenn kein Ausgaberaumbezug vorhanden ist, wird der Raumbezug der Eingabegeometrie verwendet. Andernfalls wird der Raumbezug des nativen Layers verwendet, um den in der Abfrage verwendeten Geometriepuffer zu generieren. Dieser Parameter gilt nur, wenn supportsQueryWithDistance true ist.
z.B. 100


**Parameter** *units*
Die Einheit zur Berechnung des Pufferabstands. Wenn keine Einheit angegeben ist, lautet der Standardwert esriSRUnit_Foot beim Abfragen von Feature-Services in ArcGIS Enterprise und esriSRUnit_Meter beim Abfragen von Feature-Services in ArcGIS Online. Dieser Parameter gilt nur, wenn supportsQueryWithDistance true ist.
z.B. "esriSRUnit_Foot", "esriSRUnit_Meter" , "esriSRUnit_StatuteMile", "esriSRUnit_Kilometer", "esriSRUnit_NauticalMile", "esriSRUnit_USNauticalMile" 


**Parameter** *relationParam*
Die räumliche Beziehungsfunktion, die beim Ausführen des Abfragevorgangs angewendet werden kann. Ein Beispiel für diese räumliche Beziehungsfunktion ist "FFFTTT***". 


**Parameter** *maxAllowableOffset*
Diese Option kann verwendet werden, um den maxAllowableOffset anzugeben, der zum Generalisieren von Geometrien verwendet werden soll, die von der Query-Operation zurückgegeben werden. Der maxAllowableOffset wird in den Einheiten von outSR angegeben. Wenn outSR nicht angegeben ist, wird davon ausgegangen, dass maxAllowableOffset in der Einheit des Raumbezugs der Karte vorliegt.
z.B. 2


**Parameter** *geometryPrecision*
Diese Option kann verwendet werden, um die Anzahl der Dezimalstellen in den Antwortgeometrien anzugeben, die von der Query-Operation zurückgegeben werden. Dies gilt nur für x- und y-Werte (nicht für m- oder z-Werte).
z.B. 3


**Parameter** *havingClause*
Diese Option ist eine mit outStatistics verwendete Bedingung, die das Query-Ergebnis auf Gruppen beschränkt, die die verwendete Aggregationsfunktion erfüllen. Der Parameter havingClause wird mit den Parametern groupBy und outStatistics verwendet und ermöglicht das Filtern von Ergebnissen aus outStatistics. Dieser Parameter gilt nur, wenn die Eigenschaft supportsHavingClause des layer true ist.


**Parameter** *returnIdsOnly*
Wenn true, enthält die Antwort nur ein Array von Objekt-IDs. Andernfalls ist die Antwort ein Funktionssatz. Der Standardwert ist false. Wenn Objekt-IDs angegeben sind, ist es ungültig, diesen Parameter auf "true" zu setzen.
Während die Anzahl der Features in der Feature-Set-Antwort begrenzt ist, gibt es keine Begrenzung für die Anzahl der Objekt-IDs, die in der ID-Array-Antwort zurückgegeben werden. Clients können dies ausnutzen, um alle abfragekonformen Objekt-IDs zu erhalten, indem sie returnIdsOnly=true angeben und anschließend Feature-Sets für Teilmengen von Objekt-IDs anfordern.
z.B. "false"


**Parameter** *returnCountOnly*
Wenn "true", enthält die Antwort nur die Anzahl (Anzahl der Merkmale/Datensätze), die von einer Abfrage zurückgegeben würde. Andernfalls ist die Antwort ein Feature set. Der Standardwert ist false. Diese Option ersetzt den Parameter returnIdsOnly. Wenn returnCountOnly = true ist, gibt die Antwort sowohl die Anzahl als auch den Umfang zurück. Dieser Parameter kann mit returnDistinctValues ​​verwendet werden, um die Anzahl unterschiedlicher Werte von Teilfeldern zurückzugeben.
z.B. "false"


**Parameter** *orderByFields*
Ein oder mehrere Variablen-/field-Namen, nach denen die Features/Datensätze geordnet werden sollen. Verwenden Sie ASC oder DESC für aufsteigend bzw. absteigend, nach jedem field, um die Reihenfolge zu steuern. orderByFields ist standardmäßig ASC (aufsteigende Reihenfolge), wenn <ORDER> nicht angegeben ist. orderByFields wird nur auf den Ebenen/Tabellen unterstützt, die angeben, dass supportsAdvancedQueries true ist.


**Parameter** *groupByFieldsForStatistics*
Ein oder mehrere Variablen-/field-Namen, nach denen die Werte für die Berechnung der Statistik gruppiert werden sollen. groupByFieldsForStatistics ist nur gültig, wenn der outStatistics-Parameter verwendet wird.


**Parameter** *outStatistics*
Die Definitionen für eine oder mehrere zu berechnende feldbasierte Statistiken. Dieser Parameter wird nur für Layers/Tabellen unterstützt, die angeben, dass supportsStatistics true ist. Bei Verwendung von outStatistics sind die einzigen anderen Parameter, die verwendet werden können, groupByFieldsForStatistics, orderByFields, time und where. 


**Parameter** *returnZ*
Bei "true" werden Z-Werte in die Ergebnisse aufgenommen, wenn die Features Z-Werte aufweisen. Andernfalls werden keine Z-Werte zurückgegeben. Der Standardwert ist false. Dieser Parameter gilt nur, wenn returnGeometry true ist und die hasZ-Eigenschaft des Layers true ist.
z.B. "false"


**Parameter** *returnM*
Bei "true" werden M-Werte in die Ergebnisse aufgenommen, wenn die Features M-Werte aufweisen. Andernfalls werden keine M-Werte zurückgegeben. Der Standardwert ist false. Dieser Parameter gilt nur, wenn returnGeometry true ist und die hasM-Eigenschaft der Ebene true ist.
z.B. "false"


**Parameter** *gdbVersion*
Die abzufragende Geodatabase-Version. Dieser Parameter gilt nur, wenn die isDataVersioned-Eigenschaft der Ebene wahr ist. Wenn dies nicht angegeben ist, bezieht sich die Abfrage auf die Version der veröffentlichten Karte.
z.B. SDE.DEFAULT


**Parameter** *historicMoment*
Dies ist der historische Moment, den es mit dem Query anzufragen gilt. Dieser Parameter gilt nur, wenn für den Layer die Archivierung aktiviert ist und die Eigenschaft supportsQueryWithHistoricMoment auf "true" gesetzt ist. Diese Eigenschaft wird in der Layer-Ressource bereitgestellt. Wenn HistoricMoment nicht angegeben ist, gilt die Abfrage für die aktuellen Features.
z.B. 1199145600000


**Parameter** *returnDistinctValues*
Bei "true" werden unterschiedliche Werte basierend auf den in outFields angegebenen Feldern zurückgegeben. Dieser Parameter gilt nur, wenn die Eigenschaft supportsAdvancedQueries der Ebene true ist. Dieser Parameter kann mit returnCountOnly verwendet werden, um die Anzahl unterschiedlicher Werte von Teilfeldern zurückzugeben. Stellen Sie sicher, dass Sie returnGeometry auf false setzen, wenn returnDistinctValues ​​true ist. Andernfalls werden keine zuverlässigen Ergebnisse zurückgegeben.
z.B. "false"


**Parameter** *resultOffset*
Diese Option kann zum Abrufen von Abfrageergebnissen verwendet werden, indem die angegebene Anzahl von Datensätzen übersprungen und beim nächsten Datensatz (d. h. resultOffset + 1) begonnen wird. Der Standardwert ist 0. Dieser Parameter gilt nur, wenn supportsPagination wahr ist. Sie können diese Option verwenden, um Datensätze abzurufen, die über maxRecordCount hinausgehen.
z.B. 100

**Parameter** *resultRecordCount*
Diese Option kann zum Abrufen von Query-Ergebnissen bis zum angegebenen resultRecordCount verwendet werden. Wenn resultOffset angegeben ist, dieser Parameter jedoch nicht, setzt der Karten-Service standardmäßig maxRecordCount ein. Der Höchstwert für diesen Parameter ist der Wert der maxRecordCount-Eigenschaft des layer. Der für diesen Parameter eingegebene Mindestwert darf nicht kleiner als 1 sein. Dieser Parameter gilt nur, wenn supportsPagination true ist.
z.B. 10


**Parameter** *returnExtentOnly*
Bei "true" enthält die Antwort nur die Ausdehnung der Features, die von der Abfrage zurückgegeben würden. Wenn returnCountOnly=true, gibt die Antwort sowohl die Anzahl als auch den Umfang zurück. Der Standardwert ist false. Dieser Parameter gilt nur, wenn die Eigenschaft supportsReturningQueryExtent der Ebene true ist.
z.B. "false"


**Parameter** *sqlFormat*
Der sqlFormat-Parameter kann entweder der Standard-SQL-92-Standard sein oder das native SQL des zugrunde liegenden nativen Datenspeichers verwenden. Der Standardwert ist none, was bedeutet, dass das sqlFormat vom useStandardizedQuery-Parameter abhängt.
z.B. "none", "standard", "native"


**Parameter** *datumTransformation*
Dieser Parameter wendet eine Datumstransformation an, während Geometrien in den Ergebnissen projiziert werden, wenn sich outSR vom Raumbezug des Layers unterscheidet. Beim Festlegen von Transformationen müssen Sie überlegen, welche Datumstransformation den Layer (nicht den Feature-Service) am besten auf die Eigenschaft outSR und sourceSpatialReference im Layer-Ressourcenbericht projiziert. 


**Parameter** *quantizationParameters*
Dies ist ein JSON-Objekt, das verwendet wird, um die Geometrie auf ein virtuelles Gitter zu projizieren, das wahrscheinlich Pixel auf dem Bildschirm darstellt. Zu den Eigenschaften des JSON-Objekts gehören Ausdehnung, Modus, Ursprungsposition und Toleranz.


**Parameter** *featureEncoding*
...
z.B. "esriDefault"


**Parameter** *timeRelation*
...
z.B. "esriTimeRelationOverlaps"


**Parameter** *returnTrueCurves*
...
z.B. "false"


**Parameter** *text*
...


**Parameter** *time*
...


**Parameter** *parameterValues*
...

 
**Parameter** *rangeValues*
...

