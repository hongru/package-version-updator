package-version-updator
=======================

a node-tool to deal with seajs-packages version updating

Usage
=====
touch a blank file named '.pvu' at the root of your proj.
<pre>
npm install -g package-version-updator
pvu [module_dir]
</pre>

`[module_dir]` is the path of de modified-package

<pre>
注:此工具约定
1) 项目根目录有一个名为'.pvu'的文件用于指示项目根目录
2) 此工具适用于使用seajs做模块开发的项目，工具只会分析当前修改的模块的package.json，去匹配项目内所有的模块的package.json和entry.js，找出受影响的依赖并自动修改。
3) 使用方式为 `npm install -g package-version-updator` 后，执行 `pvu [module_dir]`，比如正在当前修改模块目录， 直接`pvu ./` 即可
</pre>
