# Packages

---

| id  | Project                                                              | Version                                                                                                                            | ⚙️  | 📅     |
| --- | -------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | --- | ------ |
| 001 | [hello-emoji](https://www.npmjs.com/package/hello-emoji)             | [![npm version](https://img.shields.io/npm/v/hello-emoji.svg?style=square)](https://www.npmjs.org/package/hello-emoji)             | 🐣  | 240122 |
| 002 | [hello-ascii](https://www.npmjs.com/package/hello-ascii)             | [![npm version](https://img.shields.io/npm/v/hello-ascii.svg?style=square)](https://www.npmjs.org/package/hello-ascii)             | 🔡  | 240124 |
| 003 | [hello-random-name](https://www.npmjs.com/package/hello-random-name) | [![npm version](https://img.shields.io/npm/v/hello-random-name.svg?style=square)](https://www.npmjs.org/package/hello-random-name) | 💃  | 240130 |
| 004 | [hello-help](https://www.npmjs.com/package/hello-help)               | [![npm version](https://img.shields.io/npm/v/hello-help.svg?style=square)](https://www.npmjs.org/package/hello-help)               | 🦄  | 240204 |

### [package-001] 🐣 Hello Emoji 🐣

```tsx
import helloEmoji from "hello-emoji";

const heart = helloEmoji.heart(); // ❤️
const check = helloEmoji.check(); // ✅
const fire = helloEmoji.fire(); // 🔥
```

### [package-002] 🔡 Hello Ascii 🔢

![image](https://github.com/dusunax/packages/assets/94776135/b4d7a364-bc63-436f-8019-fe9ff050ac8e)

### [package-003] 💃 Hello Random Name 🕺

```tsx
import helloRandomName from "hello-random-name";

const randomName = helloRandomName.getName();
/*{
 *  gender: 'male',
 *  name: { english: 'Hyunseok', japanese: 'ヒョンソク', korean: '현석' }
 *}
 */
const randomFemale = helloRandomName.getName("female");
const randomMale = helloRandomName.getName("male");
const allNameList = helloRandomName.getAllNames();
```

### [package-004] 🦄 Hello Help ✨

```tsx
import { HelloHelp, helloHelpCli } from "hello-help";

const helloHelp = new HelloHelp(
  "🦄 hello-help ✨",
  "print your --help option easy",
  {
    hello: {
      optionName: "hello",
      description: "nice to say hello to you 👋",
    },
    heart: {
      optionName: "heart",
      shortenOptionName: "ht",
      description: "need a heart? 🩷",
    },
  }
);

helloHelpCli(helloHelp);
```
