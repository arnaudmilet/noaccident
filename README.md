
<!-- README.md is generated from README.Rmd. Please edit that file -->

# \#noaccident <img src="Images/no_accident.png" align="right" alt="" width="120" />

# Contexte

## Objectif

**Ambition :** proposer un cadre de vie dans lequel les flux cyclistes
sont sécurisés et des moyens sont mis en oeuvre pour systématiquement
réduire l’occurrence d’accidents impliquant des cyclistes

**Analyse a posteriori :** Identifier les zones accidentogènes d’un
territoire pour les cyclistes à travers l’analyse des flux et des
caractéristiques des lieux d’accident

**Analyse a priori :** identifier les zones susceptibles de présenter
des caractéristiques accidentogènes sur la base de l’analyse a
posteriori

**Reproductibilité :** Proposer un modèle d’analyse générique pour
permettre de réaliser l’évaluation d’un territoire par une collectivité,
une association ou des usagers avertis avec comme objectif de proposer
des évolutions de la voirie susceptible de réduire l’accidentologie

## Besoins

**T1** - Définir les caractéristiques types des zones accidentogènes à
travers l’analyse fine de la voirie, des flux, de la météo et de toutes
propriétés discriminantes

**T2 -** Identifier les zones d’un territoire géographique susceptible
de présenter des critères accidentogènes sur la base de ces critères

**Data \>** Produire un module d’analyse open-source, documenté et
partagé pour les zones accidentogènes.

**Communication \>** Promouvoir le modèle d’analyse à travers un site
internet, un github et des outils de communication à destination des
cibles identifiés

## Cibles

**1- Les collectivités** pour les aider à prioriser les investissements
dans les équipements de sécurisation de voirie des flux cyclistes sur
leurs territoires.

**2- Les associations de cyclistes** pour analyser les territoires et
appuyer leurs plaidoyers pour demander des évolutions des pratiques des
collectivités

**3- Les fournisseurs de service d’itinéraires** cyclistes pour intégrer
le contournement de zones identifiables comme plus accidentogènes dans
leurs calculs

# Les données

## Description des données disponibles

<table class="table" style="margin-left: auto; margin-right: auto;">
<thead>
<tr>
<th style="text-align:left;">
dataset
</th>
<th style="text-align:left;">
description
</th>
<th style="text-align:left;">
format initial
</th>
<th style="text-align:left;">
utilisation
</th>
<th style="text-align:left;">
Source
</th>
<th style="text-align:left;">
Disponible
</th>
<th style="text-align:left;">
Millésime
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
geovelo
</td>
<td style="text-align:left;">
Aménagement cyclable qualifiés
</td>
<td style="text-align:left;">
geojson
</td>
<td style="text-align:left;">
Visualiser les aménagements cyclables
</td>
<td style="text-align:left;">
géovélo
</td>
<td style="text-align:left;">
France
</td>
<td style="text-align:left;">
2023
</td>
</tr>
<tr>
<td style="text-align:left;">
BAAC
</td>
<td style="text-align:left;">
Data d’accidentologie sur les 13 années de 2009 à 2021
</td>
<td style="text-align:left;">
csv
</td>
<td style="text-align:left;">
localiser les accidents sur la carte à l’aide des coords GPS
</td>
<td style="text-align:left;">
onisr
</td>
<td style="text-align:left;">
France
</td>
<td style="text-align:left;">
2009 à 2021
</td>
</tr>
<tr>
<td style="text-align:left;">
osm
</td>
<td style="text-align:left;">
data openstreetmaps pour la zone LR
</td>
<td style="text-align:left;">
pbf
</td>
<td style="text-align:left;">
fond de carte et description
</td>
<td style="text-align:left;">
geofabrik
</td>
<td style="text-align:left;">
France
</td>
<td style="text-align:left;">
2014 à 2023
</td>
</tr>
<tr>
<td style="text-align:left;">
Communes
</td>
<td style="text-align:left;">
Le découpage administratif des communes françaises
</td>
<td style="text-align:left;">
rds
</td>
<td style="text-align:left;">
Ces données permettent d’effectuer des croisements avec d’autres sources
de données dans le but de construire des représentations thématiques du
territoire selon une granularité administrative (commune, arrondissement
départementaux, département, région).
</td>
<td style="text-align:left;">
insee
</td>
<td style="text-align:left;">
France
</td>
<td style="text-align:left;">
2017
</td>
</tr>
<tr>
<td style="text-align:left;">
eco-compteurs
</td>
<td style="text-align:left;">
Comptages vélo et piéton issus des compteurs de vélo
</td>
<td style="text-align:left;">
csv
</td>
<td style="text-align:left;">
</td>
<td style="text-align:left;">
Montpellier Méditerranée Métropole
</td>
<td style="text-align:left;">
Montpellier
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
FMD
</td>
<td style="text-align:left;">
Bénéficiaires du forfait mobilité durable
</td>
<td style="text-align:left;">
</td>
<td style="text-align:left;">
Reconstituer les flux domicile/travail à vélo des bénéficiaires
</td>
<td style="text-align:left;">
Université Paul Valery
</td>
<td style="text-align:left;">
Non disponible pour le moment
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
Compteurs de véhicules particuliers
</td>
<td style="text-align:left;">
Comptage véhicules particuliers de Montpellier
</td>
<td style="text-align:left;">
csv
</td>
<td style="text-align:left;">
</td>
<td style="text-align:left;">
Montpellier Méditerranée Métropole
</td>
<td style="text-align:left;">
Montpellier
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
RAMSESE
</td>
<td style="text-align:left;">
Adresse et géolocalisation des établissements d’enseignement du premier
et second degrés
</td>
<td style="text-align:left;">
geojson
</td>
<td style="text-align:left;">
Visualiser les établissement scolaires
</td>
<td style="text-align:left;">
Ministère de l’Éducation Nationale et de la Jeunesse
</td>
<td style="text-align:left;">
France
</td>
<td style="text-align:left;">
2022
</td>
</tr>
<tr>
<td style="text-align:left;">
VilleMTP_MTP_CarteScoElem
</td>
<td style="text-align:left;">
Carte scolaire des écoles élémentaires de Montpellier
</td>
<td style="text-align:left;">
shp
</td>
<td style="text-align:left;">
Associer les écoles élémentaires aux carreaux insee
</td>
<td style="text-align:left;">
Montpellier Méditerranée Métropole
</td>
<td style="text-align:left;">
Montpellier
</td>
<td style="text-align:left;">
2022
</td>
</tr>
<tr>
<td style="text-align:left;">
VilleMTP_MTP_CarteScoMat
</td>
<td style="text-align:left;">
Carte scolaire des écoles maternelles de Montpellier
</td>
<td style="text-align:left;">
shp
</td>
<td style="text-align:left;">
Associer les écoles maternelles aux carreaux insee
</td>
<td style="text-align:left;">
Montpellier Méditerranée Métropole
</td>
<td style="text-align:left;">
Montpellier
</td>
<td style="text-align:left;">
2022
</td>
</tr>
<tr>
<td style="text-align:left;">
données carroyées
</td>
<td style="text-align:left;">
La grille de niveau 200 mètres correspond à un pavage du territoire
français par des carreaux de 200 mètres de côté. Sur certains carreaux,
le nombre de ménages fiscaux peut être inférieur à 11, seuil de
confidentialité pour la source fiscale. Dans ce cas, la donnée qui est
présente dans le fichier est imputée. L’utilisateur est informé dans ce
cas par la présence d’une indicatrice I_est_200 qui est égale à 1 en cas
d’imputation.
</td>
<td style="text-align:left;">
txt
</td>
<td style="text-align:left;">
Dénombrer les enfants potentiellement cyclistes
</td>
<td style="text-align:left;">
insee
</td>
<td style="text-align:left;">
France
</td>
<td style="text-align:left;">
2017
</td>
</tr>
<tr>
<td style="text-align:left;">
OSM_Metropole_ecole_point
</td>
<td style="text-align:left;">
Lieux d’enseignement de Montpellier Méditerranée Métropole
</td>
<td style="text-align:left;">
kml
</td>
<td style="text-align:left;">
Visualiser les établissement scolaires
</td>
<td style="text-align:left;">
Montpellier Méditerranée Métropole
</td>
<td style="text-align:left;">
Montpellier
</td>
<td style="text-align:left;">
2022
</td>
</tr>
<tr>
<td style="text-align:left;">
Ensemble_temp_trajet_carreaux_200m_select_explode
</td>
<td style="text-align:left;">
Flux scolaires calculés avec openrouteservice
</td>
<td style="text-align:left;">
rds
</td>
<td style="text-align:left;">
Identifier les axes les plus utilisés par les enfants cyclistes pour se
rendre à leur école
</td>
<td style="text-align:left;">
d-sidd
</td>
<td style="text-align:left;">
France
</td>
<td style="text-align:left;">
2022
</td>
</tr>
</tbody>
</table>

## Cas pratique sur Montpellier Méditerranée Métropole

Le cas pratique que nous avons choisi de traiter est Montpellier
Méditerranée Métropole. L’ensemble des données présentées ci-dessus ont
été préparées et pré-traitées pour ce territoire.
