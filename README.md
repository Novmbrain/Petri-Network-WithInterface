PNEditor (Petri Net editor)
========

# 简介



本项目实现Petri Network的可视化。首先我们实现了Petri Network的所有功能（https://github.com/Novmbrain/Reseau-de-Petri），并在这个项目中使用适配器设计模式将自己实现的功能（上面仓库的代码）适配到现成的交互界面里。交互界面的代码是由Joris Thaveau提供的，可以从[www.pneditor.org](http://www.pneditor.org/)下载。

> Petri Network简介：https://baike.baidu.com/item/Petri%E7%BD%91/3322876

## 快速开始

1. 运行 main函数
2. 右键“change model”，选择“fuxin”，这个是我们自己的代码实现
3. 使用交互界面进行Petri Network节点，边的添加，删除等一系列操作。

## 代码构成

本项目中我们自己实现的代码在下面两个路径下：

Petri-Network-WithInterface/src/org/pneditor/petrinet/adapters/fuxin/：适配器实现

Petri-Network-WithInterface/src/org/pneditor/petrinet/models/fuxin/：Petri Network函数功能实现

# Introduction



I integrated  [my realization of Petri Network](https://github.com/Novmbrain/Reseau-de-Petri)  in this interface using the adapter's design patterns

## Quick Start

1. run main function
2. right click "Change model" and choose "fuxin"
3. start to enjoy~~~~~~~

## Originnal README

The original PNE can be downloaded from [www.pneditor.org](http://www.pneditor.org/)

This instance is the result of a student project by Joris Thaveau for teaching purpose.

It is a simplified Petri net editor that allows the editing of many PetriNet models.

To use:

1. Run org.pneditor.editor.Main as a Java application
2. Select the model used (the menu scans the org.pneditor.petrinet.adapters folder to build a list of available models and adapters). initial and imta are available. Places and transitions are displayed in different ways.
3. Edit the PetriNet and fire transitions.

You may experiment some unexpected exceptions. Especially if you mix models.

The pedagogical approach consists in:

1. Develop your own PetriNet model in an independent project/environment - with no GUI, just the ''business'' view
2. Pack it as a jar, and let it be visible in the path
3. Develop an Adapter in the org.pneditor.petrinet.adapters folder of PNE to make your model editable

The adapter may be simple or complex depending on the "distance" between your model and the one expected by PNE.

Code license: [GNU GPL v3](http://www.gnu.org/licenses/gpl.html)

Requirements: Java SE 8+
