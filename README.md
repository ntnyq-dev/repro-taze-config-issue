# repro-taze-config-issue

## Step to repro

 run `pnpm run bump`.

`taze.config.ts` is ignored. 

`html-webpack-plugin` is not excluded from bumpping.

## Workaround

Overrides `unconfig` to 0.3.13

```json
{
  "pnpm": {
    "overrides": {
      "unconfig": "0.3.13"
    }
  }
}
```
