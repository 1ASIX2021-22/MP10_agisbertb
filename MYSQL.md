<h1 align="center">
  <b>Instal·lació sistema gestor de base de dades. MySQL</b>
</h1>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155364414-9f5e788a-1d73-410c-a799-36d59c480bd3.png">
</p>
<br>
<p align="center">
  Començarem instal·lant el MYSQL Server amb la comanda <b>apt install mysql-server</b>, li indicarem que Sí.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155302043-05e4211c-d0ca-4959-94db-917f8871cf96.png">
</p>

<p align="center">
Acabarà la instal·lació donant alguns errors, però no ens afectarà a nosaltres per al que volem fer.
</p>
  
<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155302575-3ec9045c-8904-4ad1-8212-c01089af7a65.png">
</p>

<p align="center">
  Com no podrem iniciar sessió al MYSQL amb el nostre usuari, amb un <b>cat</b> veurem el contingut d'aquest fitxer on obtindrem l'usuari i password del usuari debyan-sys-maint.
</p>
  
<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155303908-2f5f1a02-661a-4218-988d-6eb4de063f8e.png">
</p>

<p align="center">
  Amb aquest usuari sí que podrem iniciar sessió, amb la següent comanda iniciarem sessió.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155304131-3461de9f-7aa5-491e-864a-e38abb11b687.png">
</p>

<p align="center">
  Un cop dins del MYSQL, crearem una base de dades de prova amb la comanda <b>CREATE DATABASE</b> i comprovarem que s'ha creat aquesta base de dades amb la comanda <b>SHOW DATABASES</b>
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155306057-bd714443-5384-4cb4-9a25-0882fe7ab05f.png">
</p>

<p align="center">
  Accedirem dins d'aquesta base de dades amb la comanda <b>use</b>, crearem una taula amb la comanda <b>create table</b> i comprovarem que s'ha creat aquesta base de dades amb la comanda <b>SHOW TABLES</b>
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155307587-e488a3a6-c8f3-420a-be5e-428da88894a0.png">
</p>

<h2 align="center">
  <b>Instal·lació i configuració MYSQL Workbench</b>
</h2>

<p align="center">
  Primer que res anirem a la pàgina de descàrregues del MYSQL Community i ens baixarem el seu repositori.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310036-c0f6bfe2-0c1e-4b7e-8f00-8bce15443fb1.png">
</p>

<p align="center">
  Accedirem dins de la carpeta <b>Baixades</b> i instal·larem aquest repositori.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310768-034e3b99-89f2-49fb-98cf-2088520743b5.png">
</p>

<p align="center">
  Escollirem la primera opció i continuarem.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310779-fa337d77-9617-4e4c-b082-9a4893374db2.png">
</p>

<p align="center">
  Aquí també escollirem la primera opció i continuarem.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310803-fb349ca9-082f-4588-a0a3-46893ba8903e.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310832-298e5d9c-1675-4e61-ab39-13b17561a022.png">
</p>

<p align="center">
  Un cop tenim el repositori instal·lat farem un apt-get update per actualitzar els repositoris.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310851-7feb10cc-dba4-42da-bb04-bdf1cca18f16.png">
</p>

<p align="center">
  Ara amb la comanda <b>apt install mysql-workbench-community</b> instal·larem aquest paquet.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310867-e71052fc-3b88-4f35-a9ab-8f95c57e600b.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155310880-78400ad2-d2d5-4d46-a239-676eb6d17473.png">
</p>

<p align="center">
  Un cop instal·lat el paquet l'iniciarem amb la comanda <b>sudo mysql-workbench</b>.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155311299-89773416-0299-4ead-864e-879675f98854.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155311321-8e5ac91e-3ea9-410a-9dc3-1f9ec3d36f03.png">
</p>

<p align="center">
  Ja dins del MYSQL Workbench farem una prova per connectar-nos a la base de dades que hem creat abans, li donarem a <b>Edit Connection</b> per editar la configuració.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155311759-4c0d4adc-14a1-46a7-af67-d554cd937bf3.png">
</p>

<p align="center">
  Per defecte l'usuari es el root però nosaltres ens connectarem amb l'usuari que hem utilitzat abans, el <b>debian-sys-maint</b>.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155312190-8e2c69c8-6170-4645-afb7-3a7ddbf278de.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155312191-bf4b69b6-d5a0-40e6-988e-dbcd348ab232.png">
</p>

<p align="center">
  Li posarem l'usuari <b>debian-sys-maint</b> i la seva contrasenya.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155313001-5035dabe-3282-42f0-b121-d0b4bfeedc70.png">
</p>

<p align="center">
  Farem un test per veure que ens podem connectar i com veiem ens funciona.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155313010-7ea8d153-0839-470b-a002-cd2dc2870420.png">
</p>

<p align="center">
  Ja som dins de la base de dades.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155313022-3f8325d2-ef86-4250-b18d-d6255cbfd519.png">
</p>

<p align="center">
  Com podem veure al lateral esquerre, si anem a <b>Schemas</b> veiem com està la base de dades i la taula que hem creat abans.
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155314088-65870cf4-7d2b-4090-ac01-657ae7d0ae9b.png">
</p>

<h2 align="center">
  <b>Configuració PHP STORM</b>
</h2>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/156244671-f5b54d5b-4a38-4971-8538-49d533674a47.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155315996-b23ee806-7463-40b4-a0ee-4b8636bc8805.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155316029-49f078fd-3eaf-4907-8807-635c45cd2bb1.png">
</p>

Ens donarà un avís que ens falten els drivers, li donarem a Download.

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155316041-7d70d924-610a-46d6-a165-b91e612190f4.png">
</p>


<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155316870-7870a4aa-11a4-4861-a795-729d3f114763.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155316845-dec9c2e5-1cbc-4734-bfa1-39fbb26f483e.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155316985-b846f4dc-4f42-4d5d-b860-e2d392d5f5f1.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155318235-d60601d9-cbd3-40d5-b871-cfd677990ef9.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155318271-4d30eeb0-4d2f-4314-b7ad-b2cc708d5791.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155318344-872b15ef-dc2d-4dda-8ed8-5f46c5ba08ad.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155339568-b8cb6559-8f7e-441f-9002-6882a13853c6.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155339582-ddc2f8c0-68da-4ebb-b9fd-19fde1d7e779.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155339591-69b487c4-55b9-443f-9f38-fa63949d5a17.png">
</p>



CODI PHP

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155319512-f0b16c68-6348-40be-b7cc-e1745c8a9f9e.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155320679-0c7001b9-dc0b-4208-a181-bcded24c7e03.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155321350-ee8c76e6-6b60-4e79-8544-6748a286f441.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155332635-b0dda926-c297-402f-aaea-9fc7d572fb7a.png">
</p>


<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155332661-22add513-5485-442d-9fb2-b70d17160fb4.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155333055-3066480b-5470-4d47-ad00-d94e669631e1.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155333063-7c8ad2ad-02f7-4e65-8fc9-91708d16a603.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155333956-f837680f-4a62-4b23-8ee1-ecd2bf978fc9.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155333972-6d510bbc-d39e-45c8-80d8-01d637a9c51d.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155333992-11a10708-371f-454c-85a5-4088d009a44b.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155334022-d54f4220-5c90-4962-81e6-a39f143c9b6a.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155335981-acc28a69-7fa7-4e22-aab0-97baebdff002.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155336052-8a9f234b-f9e1-4e91-8829-99f1bf44ddf5.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155336006-d9453e1e-bf83-46f1-83d7-a6d347036cf7.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155340040-4f5b94db-3ac4-42ec-81ca-906b0e35a479.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155340056-32c60c14-9319-4c0a-a668-f19c45063167.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155475958-79727701-d85b-4f95-8188-20733d031bd0.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476003-1e020cf2-dff2-4172-87c5-90f95ce0f811.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476088-039b4689-0344-4755-b132-9c6d882928bb.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476437-c036c992-787f-4a96-ac81-9f832cf6af1d.png">
</p>


<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476454-73138404-cd01-4be8-a3b5-640fe2c3fe8c.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476502-12a95382-24ba-49ff-8952-3dc03e56d510.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476526-8399979a-ff00-4161-943f-032cb58ee144.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476601-81d2571d-0b83-4843-88a9-02b6452c9bb5.png">
</p>

<p align="center">
  <img src="https://user-images.githubusercontent.com/91249151/155476611-08f919b2-5cbc-4868-8936-baccd459d0ac.png">
</p>
