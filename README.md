# ecomate-monorepo
Merged repository for EcoMate Application
Individual Repos :
* Web : https://github.com/Reigenleif/ecomate-web
* Mobile UI : https://github.com/Reigenleif/ecomate-mobile-ui
* Mobile Backend : https://github.com/Reigenleif/ecomate-mobile-backend-service

# Team Members
* Alif Amirudin (Hacker)
* Hanandito Pramadhan (Hustler)
* Moch. Rahadian Amantjik (Hustler)
* Ing Wening Prasetijo (Hipster)

# Application Description
EcoMate is a mobile application that provides information and resources for a sustainable
lifestyle, helping people who want to switch to a more environmentally friendly way of living. The
application offers comprehensive information about sustainable living, including
recommendations and a marketplace for environmentally friendly goods, a carbon footprint
calculator for users, and step-by-step and everyday tips to support users' journey towards living
a sustainable lifestyle. With this application, users can easily access a wealth of information and
resources to help them make more sustainable choices in their daily lives. Through this app, We
try to solve the environmental problems related to 3rd SDG : “Good Health & Well-Being”, 12th
SDG : "Responsible Consumption And Production" and also 13th SDG : “Climate Action”, as the
majority of households still lack an understanding of how to live in a more environmentally
friendly manner. There are 3 features on this application.
1. News and Tips about sustainable lifestyle
2. Marketplace for sustainable consumption
4. Carbon footprint calculator and Air Quality Index (AQI) viewer

# Future improvement
We believe that our application has more potential that can be developed in the future. We have planned these features to be added for the future improvement.
1. A sustainable lifestyle forum
2. Set target profile for sustainable (this affects general app content)
3. Using machine learning to determine carbon footprint activities based on image taken
4. Carbon tax paymen

# Architecture
This application is designed with microservice architecture with RPC as interservice communication protocol. Heres the simple diagram
<img src="https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/92985d25-cb01-4a57-9dde-d9246d5a3b76" h="300px">


# Tech used

## Backend & Database
<table>
  <tr>
    <td>
      <img src="https://academy.alterra.id/blog/wp-content/uploads/2021/07/golang-img.png" height="100px">
    </td>
    <td>
      <img src="https://grpc.io/img/logos/grpc-icon-color.png" height="100px">
    </td>
    <td>
      <img src="https://www.postgresqltutorial.com/wp-content/uploads/2012/08/What-is-PostgreSQL.png" height="100px">
    </td>
  </tr>
</table>
We use golang with gRPC as a backend, this two combines into a fast development and efficient communication machine. We also use PostgreSQL as a database.

## Mobile UI
<table>
  <tr>
    <td> 
         <img src="https://skmkuma.com/wp-content/uploads/2021/07/flutter_logo.png" height="100px"></td>
   </tr>
</table>
As our main product, we use flutter as our mobile developing framework.

## Web (Admin Dashboard)
<table>
  <tr>
    <td>
      <img src="https://indoittraining.com/wp-content/uploads/sites/3/2020/11/reactjs.png" height="100px">
    </td>
    <td>
      <img src="https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/722732dd-d64b-4a0f-84e0-c30b559a3686" height="100px">
    </td> 
    <td>
      <img src="https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/01f3f5d5-f17f-49e8-bbd0-82aca6bbfe21" height="100px">
    </td> 
    <td>
      <img src="https://seeklogo.com/images/T/trpc-logo-741E01B855-seeklogo.com.png" height="100px">
    </td>
  </tr>
</table>
We create an admin dashboard for administrators so they can manage contents easier.

# How to run
We have provided the apk file in the root dir so you can install it easely. We also provided the google cloud run hosted admin website below
[https](https://ecomate-web-hjmom73g2a-as.a.run.app/)

there's a dummy admin :
email : raha@eco.mate
password : rahadian

If you want to install manually, follow instructions provided below.

## Web application
Assume you have an active PostgreSQL database and NodeJS installed
1. Redirect to web application folder
2. Configure .env file with your DATABASE_URL and JWT_SECRET
3. Run command ```npx prisma db push```
4. Run command ```yarn dev```
5. Open your favourite browser
6. Navigate to http://localhost:3000

## Mobile UI
Assume you have installed dart and flutter, and also have a JDK installed
1. Redirect to mobile UI folder
2. Connect your phone (gRPC won't work on browser)
3. Run command ```flutter pub get```
4. Run command ```flutter run --release```

## Mobile Backend
Assume you have installed go
1. Redirect to mobille backend folder
2. Run ```go run main.go```

# Mobile Features
* Home Page
![flutter_01](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/358868f0-1be2-48a8-b561-eaf505cd4078)
![flutter_02](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/6925c669-2332-4b3d-b958-c0a024e30e92)

* Marketplace
![flutter_03](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/0036e395-f463-4142-a56e-24b127cfc347)
![flutter_04](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/1b4a0375-8c65-44d0-892e-c0beabea425c)
![flutter_05](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/cdcf51f1-f29c-4da9-ac3f-8e15ee80980a)
![flutter_06](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/50419960-bb42-48a2-aa62-b5d0c5b8a67e)

* News Page
![flutter_08](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/ba6384f5-6ad5-46c6-bb65-ae6ff87107a5)

And more...

# Web Features
* Admin Manage News
![image](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/a8e32198-bef0-44ba-8d3d-0e8029c08b4a)

* Admin Manage EcoTips
![image](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/8ba8f3ff-0276-4fbd-9e9d-2d0f5aa86e46)


* Admin Manage EcoMart items
![image](https://github.com/Reigenleif/ecomate-monorepo/assets/96337290/2ff1ca34-45f7-479e-b9f3-9a92fb9acd56)


