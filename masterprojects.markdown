---
layout: page
title: Masterprosjekter
permalink: /masterprojects/
---

<!-- TODO: distribuer til NTNU (Håvard)/OsloMet (Martin)/UiO (Kai/Martin 2021) -->
<!-- TODO: snakk med Kai om mulige UiO-masterprosjekter: Vi plukker opp denne tråden neste sommer/høst -->

Her har vi listet noen mulige masterprosjekter som kan gjøres i prosjektet Havvarsel med veiledning fra en eller flere av samarbeidspartnerne. Dette er forslag til prosjekter, hvor detaljene kan skreddersys etter interessene og bakgrunnen til den enkelte student. Av praktiske årsaker så er prosjektbeskrivelsene skrevet på engelsk. Ta kontakt så finner vi ut hva som er mulig.

# Maskinlæring

**Maskinlæring for kvalitetskontroll av brukerobservasjoner** /
**Machine learning for quality control of user observations**

Today's production of ocean forecasts is a scheduled operation with typical cycles of one day, using geophysical models that generate very large data sets. We aim to tailor the forecasts to users' specific needs by combining dedicated user observations with a subset of the traditional forecast products. Public-private partnerships and citizen observations are becoming increasingly relevant also for the conventional forecast models, which means that the ability to handle non-standard data streams from non-standard sensors are becoming increasingly important for the responsible government agencies. This requires effective and automated quality control, bias correction and aggregation of the observations. The use of machine learning models to perform automated quality control of citizen in-situ observations (either manual or from IoT-devices) is the basis of this master project.

**Maskinlæring for prediksjon av badetemperaturer (for punktvarsler)** /
**Machine learning for prediction of sea temperatures at swimming locations**

Temperatures in the upper few meters of the sea close to the coast experiences large short-time variations. Several physical processes are involved (e.g., solar heating, wind-driven on-shore and off-shore water, transports, retention areas in bays and shallow areas). Therefore, local prediction is extremely difficult. On the other side, there is a huge seasonal public interest for this information, especially the forecast options. Tourist industry and media have a need for more correct information to customers and readers, and waterfront hotels want to give these as a service to their guests. There is a growing number of sensors from both moving and fixed platforms deployed at public beaches, hotels, sea farms and harbors. The use of such observations as input to machine learning models to produce personalized local forecasts is the basis of this master project.

# Informatikk

**Forprosjekt på havvarsel.no (med universell utforming)**
<!-- TODO: fyll inn kort beskrivelse, kontaktpunkt og relevante emner -->

**Brukerstyrt drivbanesimulering på havvarsel.no (med GPU Ocean/OpenDrift/OceanParcels som backend)**
<!-- TODO: fyll inn kort beskrivelse, kontaktpunkt og relevante emner -->

# Computational statistics

**Efficient data assimilation methods for oceanographic forecasting** 
Data assimilation refers to mathematical techniques that combine predictions from a numerical model with recent available observations to obtain an improved estimate of the state of a system. In practical oceanography, we typically start forecast simulations a bit back in time and use recent real-world observations to steer the forecast to be statistically consistent with the observed values. This gives us better initial conditions for the actual forecast, which then will be more accurate and less uncertain.

Currently, we do active research both on classical ensemble Kalman filters and nonlinear particle filters for assimilation of sparse observations of ocean currents into ensembles of simplified ocean models, with focus on real-world applications. Master projects on data assimilation can, however, be more focused on algorithmic improvements of existing methods or explorations of new or tailored methods. We encourage interested students to take contact to discuss relevant project ideas.

Contact: [Håvard Heitlo Holm](https://www.sintef.no/alle-ansatte/ansatt/?empid=5205)


# Numerical mathematics

**The use of thermal rotational shallow water for ensemble drift-trajectory prediction**
The rotational shallow-water equations describe the barotropic dynamic of the ocean, meaning that they assume that the pressure is solely determined by the vertical distance from the sea surface. In a generalized circulation model, however, the pressure also depends on spatial differences in water density caused by variations in temperature and salinity, leading to barocline dynamics as well. In a recent paper, Kurganov et al [1] describe a finite-volume method for solving the so-called thermal rotational shallow-water equations, which include density as an additional variable. It can thus be used for capturing both barotropic and barocline oceanographic dynamics.

This master project would investigate the use of a GPU-accelerated thermal rotational shallow-water equations as a simplified ocean model for drift trajectory prediction and compare it against the currently used model with constant density. 

[1] Kurganov et al, 2020: https://doi.org/10.1080/03091929.2020.1774876 

Contact: [Håvard Heitlo Holm](https://www.sintef.no/alle-ansatte/ansatt/?empid=5205)


<!-- **Initialisere simulering/varsel fra NetCDF med bruk av temperatur og saltholdighet** -->
<!-- TODO: fyll inn kort beskrivelse, kontaktpunkt og relevante emner -->

<!-- **Inkludere atmosfærisk trykk (med sikte på å skape baroklin dynamikk)** -->
<!-- TODO: fyll inn kort beskrivelse, kontaktpunkt og relevante emner -->

**Efficient numerical methods for multi-layered shallow-water models for oceanographic applications**
The shallow-water equations in a rotating frame of reference model sea-level and horizontal momentum and can be used as a simplified ocean model. It is a hyperbolic system of equations which can be solved efficiently through explicit methods implemented on massively parallel hardware, such as GPUs. An obvious weakness however, is that as a 2D model, it models the momentum as an average through the water column only, meaning that it assumes the current to be the same near the surface and near the bottom. 

A slightly more realistic approach is to stack two (or more) shallow-water models on top of each other, with the bottom layer being significantly deeper and slightly denser than the upper layer. The main challenge with such models is that if the shear between the layers becomes too large, the model will no longer be hyperbolic. 
We propose a master project that would investigate how we can use a multi-layered shallow water model as a simplified model for oceanographic forecasting, with an emphasis on 

*	efficient implementation of suitable numerical methods on GPUs,
*	how to deal with (or avoid) loosing hyperbolicity in realistic applications,
*	initialization from operation models and simulation of realistic domains along the Norwegian coast.

Contact: [Håvard Heitlo Holm](https://www.sintef.no/alle-ansatte/ansatt/?empid=5205)

