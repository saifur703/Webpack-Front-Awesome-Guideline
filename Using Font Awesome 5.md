# Using Font Awesome 5 With Webpack

#### Step 1: Add fontawesome-svg-core to your project
```
yarn add --dev @fortawesome/fontawesome-svg-core
```

#### Step 2: Add the Font Awesome libraries you’ll be using
```
yarn add --dev @fortawesome/free-solid-svg-icons
```
```
yarn add --dev @fortawesome/free-regular-svg-icons
```
```
yarn add --dev @fortawesome/free-brands-svg-icons
```

#### Step 3: Import the SVGs
```
import { library, dom } from "@fortawesome/fontawesome-svg-core";
import { faCheck } from "@fortawesome/free-solid-svg-icons/faCheck";


library.add(faCheck);
dom.watch();
```
for multiple icon
```
library.add({
  faCheck,
  faAddressBook,
  faCar
});
```

#### Step 4: Add the icon to your HTML
```
<i class="fas fa-check"></i>
```
If we’ve done our job, we should see a check mark on the resulting HTML:

![](https://imgur.com/owFBqt0.png)
