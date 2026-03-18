# Suivi-des-controles
Mon application de suivi des contrôles 

<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Absences Professeurs</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf-autotable/3.5.28/jspdf.plugin.autotable.min.js"></script>

<style>
body{
  font-family:Arial;
  background:#f5f5f5;
  margin:0;
}

h1{
  text-align:center;
}

.container{
  max-width:600px;
  margin:auto;
  background:white;
  padding:15px;
  border-radius:10px;
}

input,select,button{
  width:100%;
  padding:10px;
  margin-top:8px;
}

button{
  background:#FF9800;
  color:white;
  border:none;
}

table{
  width:100%;
  margin-top:10px;
  border-collapse:collapse;
}

th,td{
  border:1px solid #ccc;
  padding:8px;
  text-align:center;
}

th{
  background:#FF9800;
  color:white;
}
</style>

</head>

<body>

<h1>Absences Professeurs</h1>

<div class="container">

<label>Date</label>
<input type="date" id="date">

<label>Nom du professeur</label>
<select id="prof">
  <option>Choisir professeur</option>
  <option>ADJE AGUIEBY JOSEPH LOUIS P.</option>
<option>AHOUMA HERVÉ</option>
<option>AKÉ N'GUESSAN PARFAIT</option>
<option>AMANKOU NÉE BROU SIALOU ARSÈNE GÉNEVIÈVE</option>
<option>ANDOH N'GUESSAN GHISLAIN-PAUL</option>
<option>ANOH PAUL EMILE</option>
<option>ASSANDE HAMIAM CESAR</option>
<option>ATTRI KOFFI JULIEN</option>
<option>BAH BI YA BLAISE</option>
<option>Balla Dembélé</option>
<option>Bamba Idrissa</option>
<option>Bandaman née Konan Ahou Clémentine</option>
<option>Biegoua Djoman Emmanuel</option>
<option>Boni Kamenan Jacques</option>
<option>Boni Nguessan Arsene</option>
<option>Brou Bangah Marcel</option>
<option>Camara née Gbané Awa</option>
<option>Cisse née Kone Fatoumata</option>
<option>Cisse Sarah Myriam</option>
<option>Cissé Ibrahima</option>
<option>Coulibaly Bakary</option>
<option>Coulibaly née Ouattara Rokia</option>
<option>Daro Djibril</option>
<option>Dey Noélie Nadège</option>
<option>Diallo Aichata</option>
<option>Diarassouba Inza</option>
<option>Diomande Sra Gouane</option>
<option>Djirieoulou Juldas</option>
<option>Eba née Kouame Ouassara Aya Jeanne</option>
<option>Eby Kouah Laurent</option>
<option>Effi Assande Eric</option>
<option>Ehoussou Hermann Michel</option>
<option>Ehui Konin Yves Pacôme</option>
<option>Essoubo Anouman Aime</option>
<option>Ettien Gnigouan Desire</option>
<option>Fadiga Mouhamed dit Douty</option>
<option>Fagoma Coulibaly</option>
<option>Fofana nee Gbahi Georgette</option>
<option>Gah epse Touré Kleon Marthe Esther</option>
<option>Gaudet Gaubaud Jean Marc</option>
<option>Gbaka Justine</option>
<option>Godehi Gnahoré Serge</option>
<option>Gomeu Minson Peguy</option>
<option>Guei Kelagnon Celestin</option>
<option>Gueu née Gogon Audrez</option>
<option>Guia Zouheudy Ghislain</option>
<option>Hugues Silvere Monnet</option>
<option>Kadjo Monson Jeanne d'Arc Epouse N'goran</option>
<option>Kamagate Adama</option>
<option>Klioua Cyrille Parfait</option>
<option>Kobenan Kra Akossua Kan Benedicte</option>
<option>Koffi Kablan Ferdinand</option>
<option>Koffi Konan Eric</option>
<option>Koffi Kouadio Anselme</option>
<option>Koko N'guessan Francois</option>
<option>Konan Kouame Williams</option>
<option>Kone Kassoum</option>
<option>Koné Lassana</option>
<option>Koné N'gorogoh Soumaila</option>
<option>Koua Anouma Cyrille</option>
<option>Kouadio Adou Thierry</option>
<option>Kouadio Epouse Yao Apo Jeannette</option>
<option>Kouadio Sery Christian</option>
<option>Kouakou Adjoumane</option>
<option>Kouakou Khofi Serge</option>
<option>Kouakou Koffi Ben</option>
<option>Kouakou Kouame David</option>
<option>Kouame Marnu Kouakou</option>
<option>Kouao Kouamé Norbert</option>
<option>Kouassi Odje Gobey Diane Marie Sylvestre</option>
<option>Kouyaté Kassoum</option>
<option>Kpla Kouadio Jean Fiacre Hermann</option>
<option>Kplohi née Diouga Mireille Joelle</option>
<option>Kra née Kahouma Nicole</option>
<option>Legbey Kouhonon Odile</option>
<option>Loba Kpassi Guillaume</option>
<option>Loukou Kouakou Urbain</option>
<option>Louoba Tiahue Adolphe</option>
<option>Mahan Hortense</option>
<option>Mel Mira Juliana</option>
<option>Mme Adom née Miézan Obrou Félicité</option>
<option>Mme Nahounou A. K. Sonia Valérie</option>
<option>Monnet Monnet</option>
<option>Monney Achiboni Romain</option>
<option>Monsekea nee Kouassi Akoua Ange</option>
<option>Monssan Eric Varèze</option>
<option>N'doua Konan Yves</option>
<option>N'guessan Kouamé Germain</option>
<option>N'guessan Kouassi Jérémi</option>
<option>Nabi Nongassida Isaac</option>
<option>Nando Oro Anne-Nathalie</option>
<option>Onamon Goua Christophe</option>
<option>Ouabio Stephane Serge</option>
<option>Ouattara Grâce Magnon Sita</option>
<option>Ouattara Yelanfi Cecile</option>
<option>Oulai Epse Yoman Keadjouhi Prudence</option>
<option>Oumar Fall</option>
<option>Ouol Lazeni Touré</option>
<option>Oussou Kouame Medard</option>
<option>Paul Yao Celestin</option>
<option>Quenum Elida Zita Valerie</option>
<option>Rebiere-Idiado Cheick Amed Andre</option>
<option>Saliou Fatahou</option>
<option>Samake Madous</option>
<option>Segui Agoh Françoise Micheline</option>
<option>Sekongo Ibrahim Kiklotialema</option>
<option>Siapo Kouassi</option>
<option>Silue Wakourgo Fanta</option>
<option>Siro Serges Hubert</option>
<option>Soffo Bertin</option>
<option>Soro Lacina</option>
<option>Soro Tchohona Valy</option>
<option>Soumahoro Seidou</option>
<option>Tano Serge</option>
<option>Tiene Mamadou</option>
<option>Touali Paulin</option>
<option>Toure Mamaro</option>
<option>Touré Bangaly</option>
<option>Touré Dramane Jean-François</option>
<option>Traore Epse Egue Mariame</option>
<option>Traore Fanta</option>
<option>Traore Ramatou</option>
<option>Yao Blé Larissa</option>
<option>Yao Dago Hubert</option>
<option>Yao Yao Alain-Claude</option>
<option>Yao Yves Cesar</option>
<option>Yatte Acho Gilles</option>
<option>Yoboue Atchelo Pascal</option>
<option>Yoboué Ahou Lucie Murielle Pulchérie</option>
<option>Zamblé Bi Boni Clermont</option>
<option>Zianeie Dethod Elodie</option>
<option>Zobo Epse Koudou Atte Felicite</option>
<option>Zoma Lydie Louise</option>
</select>

<label>Discipline</label>
<select id="matiere">
  <option>Français</option>
  <option>Anglais</option>
  <option>Espagnol</option>
  <option>Allemand</option>
  <option>Histoire/Géographie</option>
  <option>Philosophie</option>
  <option>Mathématiques</option>
  <option>Physique/Chimie</option>
  <option>SVT</option>
  <option>Arts Plastiques</option>
  <option>Musique</option>
  <option>EPS</option>
  <option>EDHC</option>
  <option>TIC</option>
</select>

<label>Classe</label>
<select id="classe">
<option>6e1</option>
<option>6e2</option>
<option>6e3</option>
<option>6e4</option>
<option>6e5</option>
<option>6e6</option>
<option>5e1</option>
<option>5e2</option>
<option>5e3</option>
<option>5e4</option>
<option>5e5</option>
<option>5e6</option>
<option>4e1</option>
<option>4e2</option>
<option>4e3</option>
<option>4e4</option>
<option>4e5</option>
<option>4e6</option>
<option>3e1</option>
<option>3e2</option>
<option>3e3</option>
<option>3e4</option>
<option>3e5</option>
<option>3e6</option>
<option>3e7</option>
<option>3e8</option>
<option>2ndeA1</option>
<option>2ndeA2</option>
<option>2ndeC1</option>
<option>2ndeC2</option>
<option>2ndeC3</option>
<option>2ndeC4</option>
<option>2ndeC5</option>
<option>1èreA</option>
<option>1èreC</option>
<option>1èreD1</option>
<option>1èreD2</option>
<option>1èreD3</option>
<option>1èreD4</option>
<option>1èreD5</option>
<option>TleA</option>
<option>TleC</option>
<option>TleD1</option>
<option>TleD2</option>
<option>TleD3</option>
<option>TleD4</option>
<option>TleD5</option>
</select>

<label>Plage horaire d'absence</label>
<select id="horaire">
  <option value="07h30-08h25">07h30-08h25</option>
  <option value="08h25-09h20">08h25-09h20</option>
  <option value="09h20-10h15">09h20-10h15</option>
  <option value="10h30-11h25">10h30-11h25</option>
  <option value="11h25-12h20">11h25-12h20</option>
  <option value="12h40-13h35">12h40-13h35</option>
  <option value="13h35-14h30">13h35-14h30</option>
  <option value="14h30-15h25">14h30-15h25</option>
  <option value="15h25-16h20">15h25-16h20</option>
</select>

<button onclick="ajouter()">Ajouter</button>
<button onclick="genererPDF()">Générer PDF</button>

<table id="table">
<tr>
  <th>Date</th>
  <th>Nom et prénoms</th>
  <th>Discipline</th>
  <th>Classe</th>
  <th>Action</th>
</tr>
</table>

</div>

<script>
let data=[];

function ajouter(){
  let date = document.getElementById("date").value;
  let prof = document.getElementById("prof").value;
  let matiere = document.getElementById("matiere").value;
  let classe = document.getElementById("classe").value;
  let horaire = document.getElementById("horaire").value;

  if(!date || prof=="Choisir professeur"){
    alert("Remplir les champs");
    return;
  }

  // Calcul de la durée de l'absence en heures
  let heures = horaire.split("-");
  let debut = heures[0].split("h");
  let fin = heures[1].split("h");

  let debutMin = parseInt(debut[0])*60 + parseInt(debut[1]);
  let finMin = parseInt(fin[0])*60 + parseInt(fin[1]);
  let dureeMin = finMin - debutMin;

  let dureeHeures = (dureeMin / 60).toFixed(2);

  data.push({
    date,
    prof,
    matiere,
    classe,
    hR: dureeHeures + " h", // heure à rattraper = durée
    hF: "" // heure rattrapée vide pour le PDF
  });

  afficher();
}

function afficher(){
  let table=document.getElementById("table");
  table.innerHTML=`
  <tr>
    <th>Date</th>
    <th>Nom et prénoms</th>
    <th>Discipline</th>
    <th>Classe</th>
    <th>Action</th>
  </tr>
  `;

  data.forEach((d,i)=>{
    table.innerHTML+=`
    <tr>
      <td>${d.date}</td>
      <td>${d.prof}</td>
      <td>${d.matiere}</td>
      <td>${d.classe}</td>
      <td><button onclick="supprimer(${i})">X</button></td>
    </tr>
    `;
  });
}

function supprimer(i){
  data.splice(i,1);
  afficher();
}

function genererPDF(){
  const { jsPDF } = window.jspdf;
  let doc=new jsPDF();
  let largeur=doc.internal.pageSize.getWidth();

  doc.text("LYCÉE MODERNE DE TREICHVILLE", largeur/2, 10, {align:"center"});
  doc.text("Année scolaire : 2025-2026", largeur/2, 16, {align:"center"});
  doc.text("SUIVI DES CONTRÔLES DE PRÉSENCE AUX COURS N°.....", largeur/2, 22, {align:"center"});

  let tableau=data.map(d=>[
    d.date,
    d.prof,
    d.matiere,
    d.classe,
    d.hR,
    d.hF
  ]);

  doc.autoTable({
    startY:30,
    head:[["Date","Nom et prénoms","Discipline","Classe","Heure à rattraper","Heure rattrapée"]],
    body:tableau
  });

  let y=doc.lastAutoTable.finalY+10;
  let today=new Date().toLocaleDateString();
  doc.text("Fait à Abidjan, le "+today, 14, y);
  doc.save("suivi_professeurs.pdf");
}
</script>

</body>
</html>
