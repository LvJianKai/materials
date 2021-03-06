# Materials

Based on fusion components and ice scaffold. [Develop material docs](https://ice.work/docs/materials/about).

## Install Deps

```bash
$ npm run setup
```

## Develop materials

```bash
# block
$ cd blocks/ExampleBlock
$ npm install
$ npm run start
```

### 自定义脚手架

scaffolds 每一个脚手架都由对应的配置文件 `.template/scaffold.json` 生成，因此请不要手动修改脚手架的其他文件内容。

生成命令：

```bash
$ cd materials/
$ node scripts/generate.js fusion-design-pro
```
### 批量发布模块

```bash
$ cd materials/
$ node scripts/publish-blocks.js
```

## Add new material

```bash
$ iceworks add  # select block|component|scaffold
```

## Generate materials data

```bash
$ iceworks generate
```

## Publish materials data

```bash
# sync to fusion material center
$ iceworks sync

# sync to oss, will work in iceworks
$ ACCESS_KEY_ID=xxx ACCESS_KEY_SECRET=yyy node scripts/oss/upload.js
```

## Use materials in iceworks

Add the materials data url to iceworks
