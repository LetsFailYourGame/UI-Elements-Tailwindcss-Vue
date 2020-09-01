## Upcoming (Work In Progress)

- desktop (hover effect)

![IMG PREV](https://www.awesomescreenshot.com/upload/1417516/1457799/19596f81-6018-49ba-53ed-07d830aca214.png "Cards")


## Small Screens Till SM Breakpoint
![IMG PREV](https://www.awesomescreenshot.com/upload/1417516/1457799/daad7543-acfb-4e05-6d7b-1413424fc9ce.png "Cards")

## Medium Till Large (Desktop) Breakpoint
![IMG PREV](http://awesomescreenshot.com/upload/1417516/1457799/b0d63b4b-7d9f-42af-7853-b3553e780cbe.png "Cards")


## Inteligent And Fast
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
## Card's Are Fully Responsive / Mobile Ready

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


