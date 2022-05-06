# PC Part Picker

## List Information

```shell
curl "https://japi.rest/pcpartpicker/v1/list/fGWxfH" \
  -H "Authorization: {API KEY}"
```

```javascript
const partId = 'fGWxfH';
const data = fetch(`https://japi.rest/pcpartpicker/v1/list/${partId}`, {
  headers: { "Authorization": "{API KEY}" }
}).then(res => res.json()).then(data => console.log(data));
```

> The above command returns JSON structured like this:

```json
{
  "cache_expiry": 3600,
  "cached": false,
  "data": [
    {
      "component": {
        "name": "CPU",
        "link": "https://pcpartpicker.com/products/cpu/"
      },
      "selection": {
        "name": "AMD Ryzen 7 3700X 3.6 GHz 8-Core Processor",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/23cd3adfd50037c1b44d6d53edb15248.256p.jpg",
        "link": "https://pcpartpicker.com/product/QKJtt6/amd-ryzen-7-3700x-36-ghz-8-core-processor-100-100000071box"
      },
      "price": {
        "base": "$269.99",
        "promo": null,
        "shipping": "FREE",
        "tax": null,
        "total": "$269.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/bhphotovideo/QKJtt6",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_bhphotovideo.png"
      }
    },
    {
      "component": {
        "name": "CPU Cooler",
        "link": "https://pcpartpicker.com/products/cpu-cooler/"
      },
      "selection": {
        "name": "NZXT Kraken X53 73.11 CFM Liquid CPU Cooler",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/098f91f23535f45875611413e7b892d6.256p.jpg",
        "link": "https://pcpartpicker.com/product/PVfFf7/nzxt-kraken-x53-7311-cfm-liquid-cpu-cooler-rl-krx53-01"
      },
      "price": {
        "base": "$119.99",
        "promo": null,
        "shipping": null,
        "tax": null,
        "total": " $119.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/amazon/PVfFf7",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_amazon.png"
      }
    },
    {
      "component": {
        "name": "Motherboard",
        "link": "https://pcpartpicker.com/products/motherboard/"
      },
      "selection": {
        "name": "MSI MPG B550 GAMING EDGE WIFI ATX AM4 Motherboard",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/e1677ccd8b20b24c91fd17885a1b8b8a.256p.jpg",
        "link": "https://pcpartpicker.com/product/2f4BD3/msi-mpg-b550-gaming-edge-wifi-atx-am4-motherboard-mpg-b550-gaming-edge-wifi"
      },
      "price": {
        "base": "$179.99",
        "promo": null,
        "shipping": null,
        "tax": null,
        "total": "$179.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/amazon/2f4BD3",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_amazon.png"
      }
    },
    {
      "component": {
        "name": "Memory",
        "link": "https://pcpartpicker.com/products/memory/"
      },
      "selection": {
        "name": "Team T-FORCE VULCAN Z 32 GB (2 x 16 GB) DDR4-3200 CL16 Memory",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/96753a64597c28e46bf80ef7064b214b.256p.jpg",
        "link": "https://pcpartpicker.com/product/TLvbt6/team-t-force-vulcan-z-32-gb-2-x-16-gb-ddr4-3200-memory-tlzgd432g3200hc16cdc01"
      },
      "price": {
        "base": "$159.99",
        "promo": null,
        "shipping": null,
        "tax": null,
        "total": "$159.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/amazon/TLvbt6",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_amazon.png"
      }
    },
    {
      "component": {
        "name": "Storage",
        "link": "https://pcpartpicker.com/products/internal-hard-drive/"
      },
      "selection": {
        "name": "Crucial MX500 500 GB 2.5\" Solid State Drive",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/d9cccb47a1d6da491f3c6e74ad51e80b.256p.jpg",
        "link": "https://pcpartpicker.com/product/ft8j4D/crucial-mx500-500gb-25-solid-state-drive-ct500mx500ssd1"
      },
      "price": {
        "base": "$57.99",
        "promo": null,
        "shipping": null,
        "tax": null,
        "total": "$57.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/amazon/ft8j4D",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_amazon.png"
      }
    },
    {
      "component": {
        "name": "Storage",
        "link": "https://pcpartpicker.com/products/internal-hard-drive/"
      },
      "selection": {
        "name": "Crucial MX500 1 TB M.2-2280 Solid State Drive",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/eca1a45c48840cfd37fd506276cda872.256p.jpg",
        "link": "https://pcpartpicker.com/product/4Qw7YJ/crucial-mx500-1tb-m2-2280-solid-state-drive-ct1000mx500ssd4"
      },
      "price": {
        "base": "$114.99",
        "promo": null,
        "shipping": "FREE",
        "tax": null,
        "total": "$114.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/adorama/4Qw7YJ",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_adorama2.png"
      }
    },
    {
      "component": {
        "name": "Storage",
        "link": "https://pcpartpicker.com/products/internal-hard-drive/"
      },
      "selection": {
        "name": "Seagate IronWolf Pro 4 TB 3.5\" 7200RPM Internal Hard Drive",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/01f719cd8e7e03916233fb39a9c5ca26.256p.jpg",
        "link": "https://pcpartpicker.com/product/vXH8TW/seagate-ironwolf-pro-4-tb-35-7200rpm-internal-hard-drive-st4000ne001"
      },
      "price": {
        "base": "$129.99",
        "promo": null,
        "shipping": "FREE",
        "tax": null,
        "total": "$129.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/bhphotovideo/vXH8TW",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_bhphotovideo.png"
      }
    },
    {
      "component": {
        "name": "Video Card",
        "link": "https://pcpartpicker.com/products/video-card/"
      },
      "selection": {
        "name": "PowerColor Radeon RX 5700 XT 8 GB Red Devil Video Card",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/529b4d648ec918d5b60553516254d871.256p.jpg",
        "link": "https://pcpartpicker.com/product/vK4BD3/powercolor-radeon-rx-5700-xt-8-gb-red-devil-video-card-axrx-5700xt-8gbd6-3dheoc"
      },
      "price": {
        "base": null,
        "promo": null,
        "shipping": null,
        "tax": null,
        "total": "No Prices Available"
      },
      "buy": {
        "link": null,
        "image": "undefined"
      }
    },
    {
      "component": {
        "name": "Case",
        "link": "https://pcpartpicker.com/products/case/"
      },
      "selection": {
        "name": "NZXT H510 ATX Mid Tower Case",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/9ee310e7133fd5145c9226f089714fa0.256p.jpg",
        "link": "https://pcpartpicker.com/product/b7hmP6/nzxt-h510-atx-mid-tower-case-ca-h510b-b1"
      },
      "price": {
        "base": "$66.98",
        "promo": null,
        "shipping": null,
        "tax": null,
        "total": "$66.98"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/amazon/b7hmP6",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_amazon.png"
      }
    },
    {
      "component": {
        "name": "Power Supply",
        "link": "https://pcpartpicker.com/products/power-supply/"
      },
      "selection": {
        "name": "Corsair RM (2019) 750 W 80+ Gold Certified Fully Modular ATX Power Supply",
        "image": "https://pcpartpicker.com//cdna.pcpartpicker.com/static/forever/images/product/02951377c9eed1e21fc3d8ba6092717e.256p.jpg",
        "link": "https://pcpartpicker.com/product/6Y66Mp/corsair-rm-2019-750-w-80-gold-certified-fully-modular-atx-power-supply-cp-9020195-na"
      },
      "price": {
        "base": "$124.99",
        "promo": null,
        "shipping": null,
        "tax": null,
        "total": "$124.99"
      },
      "buy": {
        "link": "https://pcpartpicker.com/mr/amazon/6Y66Mp",
        "image": "https://cdna.pcpartpicker.com/static/img/vendor-logos/logo2_merchant_amazon.png"
      }
    }
  ]
}
```

This endpoint retrieves a pcpartpicker list's information.

### HTTP Request

`GET https://japi.rest/pcpartpicker/v1/list/:listid`

### Path Parameters

Parameter | Required | Description
--------- | -------- | -----------
listid    | true     | The list id