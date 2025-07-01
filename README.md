
# ArtWork

ArtWork is a full-stack web application where users can explore continent-wise art events hosted in various galleries and featuring prominent artists. 
Built with React frontend, Express/Node, MongoDB database.

---

## Demo Link

[Live Demo](https://art-work-showcase.vercel.app/)

---
## Quick start

```
git clone https://github.com/KishorLangote/artWork.git
cd backend
npm install
npm run dev

cd frontend
npm install
npm run dev

```

---

## Technologies
- React JS
- Bootstrap
- React Router
- Node JS
- Express
- MongoDB

---

## Demo Video
[Loom Video](https://www.loom.com/share/0b6b3e54f08045308e07ff1c441eff7d?sid=901a3726-8586-4438-98df-8f328038bc58)

---

## Features
**Home**
- Display a list of all art Events.
- Search by gallery name or continent.
- Users can browse and filter art events based on continent Asia, Europe, and North America.

**Event Details**
- View full art event information including attached artist portfolios and artworks.

---
## API Reference

### GET /artEvents**<br>
List all art events<br>
```
Get art event response

[{
    "coordinates": {
      "latitude": 24.5333,
      "longitude": 54.4
    },
    "contactInfo": {
      "email": "info@louvreabudhabi.ae",
      "phone": "+971 2 672 1111"
    },
    "_id": "67b24458cff870aafad13c52",
    "title": "Global Art Masters Exhibition 2025",
    "date": "2025-10-05",
    "eventType": "Exhibition",
    "continent": "Asia",
    "country": "UAE",
    "city": "Abu Dhabi",
    "eventImageUrl": "https://www.gokite.travel/wp-content/uploads/2021/10/Louvre-Museum-Abu-Dhabi-Tickets-3-1-870x480.webp",
    "host": [
      "Curator",
      "Art Historian"
    ],
    "hostImageUrl": "https://www.gokite.travel/wp-content/uploads/2021/10/Louvre-Museum-Abu-Dhabi-Tickets-5-870x480.webp",
    "descriptions": "A cross-continental exhibition at the iconic Louvre Abu Dhabi, featuring masterpieces from Asian and Middle Eastern artists. Global Art Masters Exhibition 2025 (September 15–October 15, Louvre Abu Dhabi)\nThis exhibition highlights 40 artists from Asia and the Middle East, featuring Mater’s Real Illusion. Free entry, extended hours (9 AM–10 PM), and curator-led talks under Jean Nouvel’s iconic dome make it a cultural landmark.",
    "artGalleryName": "Louvre Abu Dhabi",
    "startEvent": "09:00 AM",
    "endEvent": "10:00 PM",
    "address": "Saadiyat Cultural District, Abu Dhabi, UAE",
    "googleMapImageUrl": "https://maps.googleapis.com/maps/api/staticmap?center=24.5333,54.4000&zoom=15&size=600x300&maptype=hybrid&markers=color:blue%7Clabel:L%7C24.5333,54.4000&key=YOUR_API_KEY",
    "entryFee": "Free",
    "artistCount": 40,
    "maxCapacity": 800,
    "ticketsAvailable": false,
    "sponsors": [
      "Emirates Cultural Foundation",
      "TDIC"
    ],
    "featuredArtists": [
      {
        "name": "Ahmed Mater",
        "imageUrl": "https://www.ithra.com/application/files/cache/thumbnails/678b53392ea8a2b2aa79aa1baf275362.jpg",
        "artWorkImageUrl": [
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/Artworks/Ashab-Al-Lal-Al-Ula/20240214-007-Ashab-Al-Lal-by-Ahmed-Mater.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214377&s=35eba28155547ad98bc6b552f8fbec0a",
            "title": "Real Illusion",
            "_id": "67b24458cff870aafad13c54"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/Artworks/Mecca-Windows-2013/AhmedMater_PreviewDinner_BM_byHT-6665.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214600&s=7b02e6a4ce0888c23476726e7d6417c1",
            "title": "Mecca Windows",
            "_id": "67b24458cff870aafad13c55"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/Artworks/100-Found-Objects-2014/1.-The-Black-Stone.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214361&s=53aa2b7c9dd29618d8d87702f52a0a87",
            "title": "The Black Stone",
            "_id": "67b24458cff870aafad13c56"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/02_fulgurite_Tesla-_Coil_scalpture_Ahmed_mater_02.82.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214205&s=75266e8aa55b2426337ac97d3c1689f0",
            "title": "02_fulgurite, 82",
            "_id": "67b24458cff870aafad13c57"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/08_fulgurite_Tesla-_Coil_scalptur_Ahmed_mater_.103.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214224&s=4ebfb7b9a6a15c23c0d18c0596086d1d",
            "title": "08_fulgurite, 103",
            "_id": "67b24458cff870aafad13c58"
          }
        ],
        "_id": "67b24458cff870aafad13c53",
        "bio": "Ahmed Mater is a Saudi Arabian artist and physician whose work critically examines socio-political and cultural narratives in the Middle East. Known for installations like Mecca Windows and The Black Stone, Mater employs mixed media to explore themes of urbanization, spirituality, and identity. A leading voice in contemporary Arab art, his practice bridges traditional Islamic motifs with modern conceptual frameworks."
      }
    ],
    "tags": [
      "Middle Eastern Art",
      "Contemporary",
      "Cultural Fusion"
    ],
    "officialWebsite": "https://www.louvreabudhabi.ae/ar/",
    "createdAt": "2025-02-16T20:02:32.890Z",
    "updatedAt": "2025-02-16T20:02:32.890Z",
    "__v": 0,
    "hostBy": [
      "Poet",
      "Artist",
      "Sculpture"
    ]
  }]
```
### GET /artEvents/artist/:artistName**<br>
Get the art work by artist name<br>
```
reponse

[{
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/Artworks/Ashab-Al-Lal-Al-Ula/20240214-007-Ashab-Al-Lal-by-Ahmed-Mater.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214377&s=35eba28155547ad98bc6b552f8fbec0a",
            "title": "Real Illusion",
            "_id": "67b24458cff870aafad13c54"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/Artworks/Mecca-Windows-2013/AhmedMater_PreviewDinner_BM_byHT-6665.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214600&s=7b02e6a4ce0888c23476726e7d6417c1",
            "title": "Mecca Windows",
            "_id": "67b24458cff870aafad13c55"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/Artworks/100-Found-Objects-2014/1.-The-Black-Stone.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214361&s=53aa2b7c9dd29618d8d87702f52a0a87",
            "title": "The Black Stone",
            "_id": "67b24458cff870aafad13c56"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/02_fulgurite_Tesla-_Coil_scalpture_Ahmed_mater_02.82.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214205&s=75266e8aa55b2426337ac97d3c1689f0",
            "title": "02_fulgurite, 82",
            "_id": "67b24458cff870aafad13c57"
          },
          {
            "imageUrl": "https://ahmed-mater.transforms.svdcdn.com/production/uploads/08_fulgurite_Tesla-_Coil_scalptur_Ahmed_mater_.103.jpg?w=1140&q=80&auto=format&fit=clip&dm=1739214224&s=4ebfb7b9a6a15c23c0d18c0596086d1d",
            "title": "08_fulgurite, 103",
            "_id": "67b24458cff870aafad13c58"
          }]
```

### GET /artEvents/title/:artEventTitle**<br>
Get art event title

---

## Contact
For bugs or feature request, please react out to kishorlangote2@gmail.com

