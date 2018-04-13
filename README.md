
# GNDecoration é um projeto de decoração simples para aplicações javaFx.

![demo1](src/main/resources/screenshot/demo1.png)


# Estrutura - Nodes

        root -> SstackPane
                body -> AnchorPane
                        top_left -> Path
                        top_right -> Path -- rotation 90°
                        bottom_left -> Path -- rotation 270°
                        bottom_right -> Path -- rotation 180°

# Estrutura - Objetos

        GNWindowProto - Fornece um protótipo inicial como um modelo para sua implementação personalizada |
        GNWindowBar   - Fornece um protótipo inicial com uma barra de ferramentas basica



<<<<<<< HEAD
## Primary Structure
=======
# Etrutura - by Scenic View
## Primary
>>>>>>> 8e13e4dc3228a307b25d397e4eadb80ca88fba21
![Structure](src/main/resources/screenshot/primarySctructure.png)

### No metódo main utilize |  In method main
  
    // init proto
    GNWindowProto decoration = new GNDecorationProto();
    decoration.show();
    
    // init proto bar
    GNWindowBar decoration = new GNWindowBar();
    decoration.setContent(node);
    // para vers as barras de redimensionamento
    decoration.viewBars(true);
    decoration.show();


# Features
* Shadow <br>
        Decoração com sombra (É possivel fazer, porém no caso do windows causa lentidaão na gui), mais no caso do linux parace não haver essa lentidão.
        Em caso de janelas pequenas utilize, exemplo decoration.setShadow(true);

# Bugs
* Cursor não aparece bem por causa do espaço limitado dentro do path no node. (porém não inpede nada só é chato) :D;