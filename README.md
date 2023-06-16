<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Oñemoñeꞌe oñemboguapy raẽ hag̃ua nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) , ha upéi `direnv allow` ojeike rire kundahárape ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) ojejapóta ijeheguiete ojeike rire kundahárape).

He’iséva ha’e: Chino ñembohasa japonés, coreano, inglés, inglés ñembohasa opaite ambue ñe’ẽme. Reipytyvõséramo chino ha inglés-pe añoite, ikatu rehai añoite `zh: en` .

He’iséva ha’e: Chino ñembohasa japonés, coreano, inglés, inglés ñembohasa opaite ambue ñe’ẽme. Reipytyvõséramo chino ha inglés-pe añoite, ikatu rehai añoite `zh: en` .

* [código tenondegua](https://github.com/xxai-art/web)
* [Ñe’ẽ ryru tenda tuichakue javeve g̃uarã](https://github.com/xxai-art/web/tree/main/i18n)
* [Ñe’ẽ ryru umi módulo jeikerãme g̃uarã](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Página web Kuatiahaipyre heta ñe’ẽme](https://github.com/xxai-doc)

Pe lenguaje programación tenondegua haꞌehína [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , omoĩva peteĩ mbaꞌeporã oñemopyendáva coffeescript ñeꞌeryru rehe, ehecha [./coffee_plus.md](./coffee_plus.md) .

## Internacionalización página web ha kuatiakuéra rehegua

Oñemopu’ã ko’ã 3 proyecto rehe

* [@w5/mdt rehegua](https://www.npmjs.com/package/@w5/mdt)

  Ñe’ẽpehẽtai ha’e `.mdt` , ikatu reipuru ñe’ẽjoaju ojoguáva `<+ ./coffee_plus/import.js>` reñe’ẽ hag̃ua vore okapegua rehe, ha emoheñói markdown ñe’ẽpehẽtai `.md` reheve.

* [@w5/trmd rehegua](https://www.npmjs.com/package/@w5/trmd)

  Markdown ñembohasa nombohasamoꞌãi umi código ha enlace, ha omoĩta caché-pe ñeꞌejoaju oñembohasáva. Oñemoambuéramo pe traduksión péro noñemoambuéi pe téxto orihinál, ojejapo jeýramo ndojeskrivimoʼãi pe traduksión oñemoambuéva.

* [@w5/i18n rehegua](https://www.npmjs.com/package/@w5/i18n)

  Umi archivo ñe’ẽ rehegua oñembohasa hag̃ua umi página web `yaml` omoheñóiva.

### Kuatia Ñembohasaha Automatización rehegua Ñe’ẽmondo

Ehecha kódigo ryru [xxai-art/doc](https://github.com/xxai-art/doc)

Oñemoñeꞌe oñemboguapy raẽ hag̃ua nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) , ha upéi `direnv allow` ojeike rire kundahárape ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) ojejapóta ijeheguiete ojeike rire kundahárape).

Ani hag̃ua ojejapo base de código tuicháva oñembohasáva hetaiterei ñe’ẽme, ajapo peteĩ base de código aparte peteĩteĩva ñe’ẽme g̃uarã ha amoheñói peteĩ organización oñongatu hag̃ua base de código

Oñemohenda ramo mba’e’oka tekoha `GITHUB_ACCESS_TOKEN` ha upéi emongu’évo [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) omoheñóita ijeheguiete kódigo ryru.

Añetehápe, ikatu avei remoĩ peteĩ base de código-pe.

Ñe’ẽasa script ñe’ẽmondo [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Pe script código oñeinterpreta kóicha:

[bunx](https://bun.sh/docs/cli/bunx) haꞌehína peteĩ npx ñemyengovia, ipyaꞌevéva. Añetehápe, ndorekóiramo bun oñemboguapýva, ikatu reipuru `npx` hendaguépe.

`bunx mdt zh` ohechauka `.mdt` zh ryru’ípe `.md` ramo, ehecha umi 2 vore ojoajúva iguýpe

* [ka’a_have.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [ka’a_ha’evéva.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` haꞌehína kódigo núcleo ñembohasarã (oguerekóramo `nodejs` añoite oñemboguapýva, ha katu `bun` ha `direnv` noñemoĩri, ikatu avei emonguꞌe `npx i18n` embohasa hag̃ua).

Ohesa’ỹijóta [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , `i18n.yml` ñemboheko ko kuatiaroguépe ha’e kóicha:

```
en:
zh: ja ko en
```

He’iséva ha’e: Chino ñembohasa japonés, coreano, inglés, inglés ñembohasa opaite ambue ñe’ẽme. Reipytyvõséramo chino ha inglés-pe añoite, ikatu rehai añoite `zh: en` .

Ipahaitéva haꞌehína [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , oguenohẽva mbaꞌe oĩva título principal ha subtítulo peteĩha apytépe peteĩteĩva ñeꞌepy `README.md` omoheñói hag̃ua peteĩ jeike `README.md` . Pe código ningo isencilloiterei, ikatu remaña ndete voi hese.

Google API ojepuru ñembohasa isãsóvape g̃uarã. Ndaikatúiramo reike Google-pe, emohenda ha emohenda peteĩ proxy, ha’eháicha:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Pe script ñembohasa rehegua omoheñóita peteĩ caché oñembohasáva `.i18n` ryru’ípe, ehechamína `git status` reheve ha emoĩ kódigo ryru’ípe ani hag̃ua ojejapo jey jey ñembohasa.

Emomba’apo `bunx i18n` opaite jave emoambue ñembohasa embopyahu hag̃ua caché.

Oñemoambuéramo peteĩ jave jehaipyre ypykue ha ñembohasa, oñembojoavyva’erã caché, upévare remoambueséramo, ikatu remoambue peteĩnte, ha upéi emongu’e `bunx i18n` embopyahu hag̃ua caché.
