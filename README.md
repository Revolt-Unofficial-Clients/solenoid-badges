# solenoid-badges

A nice way to manage and add badges to any third party client.

## Setup

```bash
git submodule add https://github.com/Revolt-Unofficial-Clients/solenoid-badges /lib/badges
```
```ts
// Import Badges from Submodule
import {badges} from "/lib/badges"

// Import Badge Types
import type {SolenoidBadge} from "/lib/badges"

badges.forEach((badge) => {
    badge.id.forEach((id) => {
        if (message.author_id === id) {
            // Do something
        }
    })
});
```

## Updating

```bash
git submodule update --remote
```

## Spec

```json
[
    {
        "id": [],
        "title": "",
        "bkg": "",
        "colour": "",
        "url": ""
    }
]
```

`id`: User IDs
`title`: Badge Name
`bkg`: Badge Background
`colour`: Badge Foreground
`url`: CORS Enabled Image/Gif URL
