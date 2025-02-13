# Gléasanna

Chun sonraí a bhailiú ag gníomhaire seachtrach, ní mór gléasanna a chruthú le paraiméadair shonraithe. Tá na gléasanna ceangailte le raca; gan nasc, ní féidir iad a chruthú. De réir réamhshocraithe, níl aon ghléasanna ann.

### **Tábla Gléasanna**

• Cuardach — cuir isteach siombailí chun scagadh de réir clibe sócmhainne.

• Ionad Sonraí, Seomra, Raca — scagairí chun gléasanna a roghnú i gceantair áirithe.

• Cruthaigh Gléas Nua — cnaipe chun gléas a chruthú.

### **Réimsí na Tábla**

• ID an Ghléis — uimhir uathúil an chórais.

• Múnla — sainmhínítear ag an ngníomhaire nó de láimh; taispeántar an firmware.

• Ráta Haisia — feidhmíocht reatha (TH/s):

🟢 Ciorcal Glas — ráta haisia níos mó ná 0.

🔴 Ciorcal Dearg — ráta haisia = 0 nó neamhshainithe.

• Ainm an Oibrí — ainm an linne agus an ghléis (sainmhínítear ag an ngníomhaire nó de láimh).

• Seoladh IP — braitear go huathoibríoch nó socraítear de láimh.

• S/N — uimhir sraitheach, braite ag an ngníomhaire nó socraithe de láimh.

• Suíomh — Ionad Sonraí / Seomra / Raca (nascanna le háiteanna).

• Nuashonrú — cnaipe chun paraiméadair a shocrú.

<figure><img src="../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

## **Cruthú Gléis tríd an bhFoirm**

1\. Téigh go **Gléasanna**.

2\. Cliceáil ar **Cruthaigh Gléas Nua**.

3\. Sa fhuinneog a osclaítear, iontráil na sonraí seo:

• **Cineál Gléis** — múnla (roghchlár anuas le cuardach). _Riachtanach._

• **Clib Sócmhainne** — ainm uathúil an ghléis sa chóras Hashcare. _Riachtanach._

• **Uimhir Sraithe** — _Riachtanach._

• **Seoladh IP** — caithfidh sé an patrún seo a leanúint:\
^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$. _Riachtanach._

• **Seoladh MAC** — caithfidh sé an patrún seo a leanúint: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$.

• **Uimhir Sceilf** — uimhir sceilf saor i raca áirithe.

* Ní féidir a bheith = 0. _Earráid: “Caithfidh sé a bheith ≥ 1”._
* Ní féidir a bheith níos mó ná líon na sceilfeanna sa raca. _Earráid: “error.codes.rack\_exceed\_max\_size”._
* Ní mór gur uimhir í. _Earráid: “Formáid neamhbhailí”._

• **Uimhir Áite** — uimhir shuíomh saor ar sceilf.

* Ní féidir a bheith = 0. _Earráid: “Caithfidh sé a bheith ≥ 1”._
* Ní féidir a bheith níos mó ná líon na suíomhanna ar an sceilf.
* Ní mór gur uimhir í. _Earráid: “Formáid neamhbhailí”._

• **URLanna Stratum an Linn** — suas le 3 URL. _Neamhobligáideach._

• **Ainm Oibrí an Linn** — ainm an ghléis ar an linn. _Riachtanach._

• **Ainm an Linne** — ainm an linne. _Riachtanach._

• **Raca** — rogha ó na racaí atá ann. _Riachtanach._

• **Cineál Firmware** — _Riachtanach._

4\. Cliceáil **Cruthaigh**.

<figure><img src="../../.gitbook/assets/image (27).png" alt="" width="446"><figcaption></figcaption></figure>

## **Iompórtáil Gléasanna mar Liosta** <a href="#importirovanie-ustrojstv-spiskom" id="importirovanie-ustrojstv-spiskom"></a>

1. Téigh go **Gléasanna**.
2. Roghnaigh **Iompórtáil Gléasanna (.csv)** sa roghchlár anuas.
3. Roghnaigh comhad .csv ar do thiomántán crua.
4. Má éiríonn leis an uaslódáil, taispeánfar an teachtaireacht **“D’éirigh leis an uaslódáil”**.

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

**Sampla Tábla CSV**

<figure><img src="../../.gitbook/assets/Снимок экрана 2024-12-19 в 23.34.15.png" alt=""><figcaption></figcaption></figure>

## **Nuashonrú Gléis**

1\. Cliceáil ar an gcnaipe (_trí phonc_) in aice leis an ngléas atá uait.

2\. Roghnaigh **Nuashonraigh**.

_**Paraiméadair in-athraithe:**_

• **Cineál Gléis** — múnla. Oibríonn an réimse mar roghchlár anuas le cuardach de réir siombailí. _Riachtanach._

• **Clib Sócmhainne** — ainm uathúil an ghléis sa chóras Hashcare. _Riachtanach._

• **Uimhir Sraithe** — _Riachtanach._

• **Seoladh IP** — caithfidh sé an patrún seo a leanúint:\
^(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9]).(25\[0-5]|2\[0-4]\[0-9]|1\[0-9]{2}|\[1-9]?\[0-9])$.\
&#xNAN;_&#x52;iachtanach._

• **Seoladh MAC** — caithfidh sé an patrún seo a leanúint: ^\[a-fA-F0-9]:\[a-fA-F0-9]{2}{5}$. _Riachtanach._

• **Uimhir Sceilf** — uimhir sceilf saor i raca sonraithe.

* Ní féidir a bheith = 0. _Earráid: “Caithfidh sé a bheith ≥ 1.”_
* Ní féidir a bheith níos mó ná líon na sceilfeanna sa raca. _Earráid: “error.codes.rack\_exceed\_max\_size.”_
* Ní mór gur uimhir í. _Earráid: “Formáid neamhbhailí.”_

• **Uimhir Áite** — uimhir shuíomh saor ar sceilf.

* Ní féidir a bheith = 0. _Earráid: “Caithfidh sé a bheith ≥ 1.”_
* Ní féidir a bheith níos mó ná líon na suíomhanna ar an sceilf.
* Ní mór gur uimhir í. _Earráid: “Formáid neamhbhailí.”_
* _Riachtanach._

• **URLanna Stratum an Linn** — suas le 3 sheoladh stratum is féidir a chur leis. _Neamhobligáideach._

• **Ainm Oibrí an Linn** — ainm an ghléis ar an linn. _Riachtanach._

• **Ainm an Linne** — ainm an linne. _Riachtanach._

• **Raca** — rogha ó na racaí atá ann. _Riachtanach._

• **Cineál Firmware** — _Riachtanach._

• **Athraigh líon na sceilfeanna** (**Airde**) — ní mór dó a bheith ≥ 1 agus ≤ 10.

• **Athraigh líon na suíomhanna in aghaidh na sceilfe** (**Leithead**) — ní mór dó a bheith ≥ 1 agus ≤ 10.

• **Athraigh an Seomra**, a mbeidh an raca ceangailte leis.

<figure><img src="../../.gitbook/assets/image.png" alt="" width="446"><figcaption></figcaption></figure>

3\. Cliceáil **Nuashonraigh** chun na hathruithe a shábháil.

## **Nuashonrú Gléasanna trí Chomhad CSV** <a href="#redaktirovanie-ustrojstv-cherez-csv-fajl" id="redaktirovanie-ustrojstv-cherez-csv-fajl"></a>

Is féidir níos mó ná aon ghléas amháin a nuashonrú ag an am céanna trí chomhad CSV a úsáid. Ní mór comhad a uaslódáil le liosta gléasanna atá ann cheana féin.

1. Is é **Seoladh MAC** an t-aithneoir príomhúil – má tá an MAC san fheiste agus sa chomhad CSV mar an gcéanna, athrófar na sonraí eile de réir an chomhaid CSV.
2. Mura bhfuil an MAC sa chóras Hashcare, cruthófar gléas nua leis na paraiméadair sa chomhad CSV.

## **Scriosadh Gléis:**

1. Cliceáil ar an gcnaipe (_trí phonc_) in aice leis an ngléas atá uait.
2. Roghnaigh **Scrios**.
3. Sa fhuinneog a osclaítear, cliceáil ar an gcnaipe **Deimhnigh**.

<figure><img src="../../.gitbook/assets/image (1).png" alt="" width="343"><figcaption></figcaption></figure>

## **Sonraí an Ghléis:**

• **Múnla**

Braitear go huathoibríoch é ag an ngníomhaire inmheánach nó socraítear de láimh é i socruithe an ghléis. Cuimsíonn sé an ráta haisia sonraithe ag an monaróir.

• **Seoladh IP**

Braitear go huathoibríoch é ag an ngníomhaire inmheánach nó socraítear de láimh é i socruithe an ghléis.

• **Firmware**

Braitear go huathoibríoch é ag an ngníomhaire inmheánach nó socraítear de láimh é i socruithe an ghléis.

• **Uimhir Sraithe (S/N)**

Braitear go huathoibríoch é ag an ngníomhaire inmheánach nó socraítear de láimh é i socruithe an ghléis.

### **Cumhacht**

• **Cumhacht Ainmnithe**

Luach statach atá socraithe do gach múnla gléis.

* W/TH - luach coibhneasta, á ríomh mar an cóimheas idir an tomhaltas ainmniúil agus an ráta haisia ainmniúil.

• **Ráta Haisia Ainmnithe**

Luach an ráta haisia a shocraíonn an monaróir agus a bhraitear ón ASIC.

### **Eolas Breise**

• **Ainm Oibrí**

Comhdhéanta d’ainm an linne agus ainm an ghléis ar an linn. Braitear go huathoibríoch é nó socraítear de láimh é i socruithe an ghléis.

• **Seoladh MAC**

Braitear go huathoibríoch é ag an ngníomhaire inmheánach nó socraítear de láimh é i socruithe an ghléis.

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### **Táscairí:**

**• Ioncam Measta (PPS | FPPS):**

* PPS (Pay Per Share): íocaíocht sheasta in aghaidh na scaireanna.
* FPPS (Full Pay Per Share): cuimsíonn sé ioncam ó tháillí, níos airde ná PPS.

**• Ioncam ón Linn:**

Ioncam iarbhír ón linn don tréimhse roghnaithe.

_Le haghaidh cumraíochta an linne: “Socruithe Linn” → Cruthaigh Linn._

**• Costais Leictreachais:**

Bunaithe ar chumhacht an ghléis agus an ráta:

(Tomhaltas Cumhachta (W) × 24) ÷ 1000 × Ráta

**• Brabús:**

{Ioncam FPPS} - {Costais Leictreachais}

### **Cairt Ráta Haisia**

• **Asic Hashrate** — ráta haisia reatha ón ngléas.

• **Nominal Hashrate** — ráta haisia sonraithe ag an monaróir.

### **Cairt Ráta Haisia Pláta**

Taispeánann sé feidhmíocht na bplátaí aonair in ASIC miner.

• Déantar gach pláta a ainmniú, m.sh., SM 0, SM 1, SM 2.

• Cabhraíonn sé le fabhtanna a aithint a d’fhéadfadh cur isteach ar an ráta haisia iomlán.

### **Teocht an Ghléis**

• Teocht na bplátaí (boards) agus na sliseanna (chip, PCB).

• Teocht an aeir (in/out):

* **In** — teocht an aeir fuar ag dul isteach.
* **Out** — teocht an aeir téite ag dul amach.

### **Cairt Luas an Lucht leanúna**

Taispeánann sé RPM (rothlacha in aghaidh an nóiméid) lucht leanúna fuaraithe.

* **In** — lucht leanúna ar an taobh ionchuir.
* **Out** — lucht leanúna ar an taobh aschuir.

### **Cairt Tomhaltas Cumhachta**

* **Asic Power** — tomhaltas reatha, seolta ag an ngléas.
* **Nominal Power** — tomhaltas sonraithe ag an monaróir.

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>
