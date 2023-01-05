This is a really simple repo meant for testing the impacting of server components on one huge component

## Testing

* run `rm -rf .next && npm run build && npm start`
* Access `http://localhost:3000/test-server-components`
* Open Devtools
* Go to Network tab
* Filter by `_next`
* Check the amount of JS loaded (probably around 227Kb)
* Open `app/test-server-components/HugeComponent.tsx` and remove `"use client"`
* Repeat the entire proccess and check the JS size again (probably around 284Kb)

***fyi***: the chunk which changes begings with `page-`

