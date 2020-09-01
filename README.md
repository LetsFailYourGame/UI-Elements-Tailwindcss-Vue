# Upcoming

- small screens and tablets

![IMG PREV](https://s3.amazonaws.com/awesomescreenshot/upload/1417516/1457799/8e25534b-7d14-438a-4da3-bebecbe8d052.png?AWSAccessKeyId=AKIAJSCJQ2NM3XLFPVKA&Expires=1599003753&Signature=DPGWn00qTNgv%2BoVR8SNrhT7vUcw%3D "Cards")


- desktop (hover effect)

![IMG PREV](https://www.awesomescreenshot.com/upload/1417516/1457799/19596f81-6018-49ba-53ed-07d830aca214.png "Cards")

# Small Screens Till SM Breakpoint
![IMG PREV](https://www.awesomescreenshot.com/upload/1417516/1457799/8a25a538-3cc9-43bf-4259-3f06aa6d59a6.png "Cards")

# Inteligent And Fast
- the data for the card's is stored in an array insided app.vue
- vue will then create as many card's as there's data
- the card's only show until **SM** breakpoint is triggered ([tailwindcss docs](https://tailwindcss.com/docs/breakpoints#app))

```javascript
 data() {
    return {
      Apartments: [
        {
          title: 'Manhattan Tower in NYC',
          img_link: 'https://images.unsplash.com/....',
          baths: 4,
          rooms: 8,
          size: 560,
          cost: 1250,
          per: 'Week',
          rating: 4,
          reviews: 256,
          description: 'The Presidio Residences on ...',
        },
        ....
     ]
```
# Card's Are Fully Responsive And Mobile Ready

![IMG PREV](https://s3.amazonaws.com/awesomescreenshot/upload/1417516/1457799/10e1acef-3c58-4441-4e8e-f73881eea543.png?AWSAccessKeyId=AKIAJSCJQ2NM3XLFPVKA&Expires=1598948943&Signature=qdazsdnEiJiLADc0O5eTybNht%2Fo%3D "Title")

### Install Vue-Cli
```
npm install -g @vue/cli
# OR
yarn global add @vue/cli
```
### Start Lokal Dev Server
```
npm run serve
```
### More Info's [[Vue-CLI](https://cli.vuejs.org/)] [[tailwindcss](https://tailwindcss.com/docs/installation)]


