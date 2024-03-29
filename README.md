# Font awesome compatible icons

This repository collects converted icon sets to use them with FontAwesome tools. All included icon sets are licensed under MIT license.

The following sets are included:

| Set | Prefix | Count | Version | Docs |
| --- | --- | ---:| --- | --- |
| [UiKit Icons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/uk.html) |`uk` | 143 | 3.10.0 | https://getuikit.com/docs/icon |
| [Feather Icons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/fi.html) |`fi` | 286 | 4.28.0 | https://feathericons.com |
| [Bootstrap Icons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/bi.html) |`bi` | 1325 | 1.7.2 | https://icons.getbootstrap.com/ |
| [Tabler Icons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/tb.html) |`tb` | 1262 | 1.51.0 | https://tablericons.com |
| [IonIcons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/ion.html) |`ion` | 1332 | 5.5.4 | http://ionicons.com/ |
| [JAM Icons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/jam.html) |`jam` | 896 | 2.0.0 | https://jam-icons.com |
| [Line Awesome Icons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/la.html) |`la` | 1544 | 1.3.0 | https://icons8.com/line-awesome |
| [Pixelart Icons](https://htmlpreview.github.io/?https://github.com/lmeysel/fa-compatible-icons/blob/master/_sprites/pa.html) |`pa` | 460 | 1.5.0 | https://pixelarticons.com/ |


## Usage

Install repository
`npm i -D https://github.com/lmeysel/fa-compatible-icons.git`

And use icons with the [known FontAwesome tools](https://fontawesome.com/how-to-use/on-the-web/advanced/svg-javascript-core#comparing):

```typescript
import { library } from '@fortawesome/fontawesome-svg-core'
import { biUser } from 'fa-compatible-icons/bi'

library.add(biUser)
```

When using e.g. [vue-font-awesome](https://github.com/FortAwesome/vue-fontawesome) it is easily possible using the icons with the corresponding prefix:

```vue
<font-awesome-icon :icon="['bi', 'user']" />
```

## Bundle size

Keep in mind that all icon sets contain many icons but you probably do not need the most of them. Therefore it is strongly recommended to use the `library.add(...)`-syntax before, in order to only add the icons to your bundle you really need.