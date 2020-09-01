# (more follow soon)

# Small Screens till SM Breakpoint
![IMG PREV](https://www.awesomescreenshot.com/upload/1417516/1457799/8a25a538-3cc9-43bf-4259-3f06aa6d59a6.png "Cards")

# Responsive and Inteligent
The Data For The Card's Is Stored In An Array Insided App.vue. Vue Will Then Create As Many Card's As There's Data. The Card's Only Show Until **sm** Breakpoint Is Triggered.

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
# Card's are fully responsive and mobile ready

![IMG PREV](https://s3.amazonaws.com/awesomescreenshot/upload/1417516/1457799/10e1acef-3c58-4441-4e8e-f73881eea543.png?AWSAccessKeyId=AKIAJSCJQ2NM3XLFPVKA&Expires=1598948943&Signature=qdazsdnEiJiLADc0O5eTybNht%2Fo%3D "Title")

# Install Vue-Cli
```
npm install -g @vue/cli
# OR
yarn global add @vue/cli
```
# Start Lokal Dev Server
```
npm run serve
```
# More Info's @ [Vue-CLI](https://cli.vuejs.org/)



