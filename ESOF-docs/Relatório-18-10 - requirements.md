# GeoTools
 
## Use Cases
        Supports OGC Grid Coverage implementation ()
        Coordinate reference system and transformation support
        Symbology using OGC Styled Layer Descriptor (SLD) specification
        Attribute and spatial filters using OGC Filter Encoding specification
        Supports graphs and networks
        Java Topology Suite (JTS) - with support for the OGC Simple Features Specification - used as the geometry model for vector features.
        A stateless, low memory renderer, particularly useful in server-side environments
        Powerful “schema assisted” parsing technology using XML Schema to bind to GML content
        Interact with OGC web services with both Web Map Server and Web Feature Server support
        Open plug-in system allowing you to teach the library additional formats
        Plug-ins for the ImageIO-EXT project allowing GeoTools to read additional raster formats from GDAL
       
## Procedimento para adiconar novas funcionalidades (features)
No GeoTools as novas funcionalidades são adicionadas ao projeto através de módulos.
Os módulos só podem ser desenvolvidos pelos Module Maintainers.
Os Module Maintainers são os contribuidores mais importantes, uma vez que desenvolvem novas funcionalidades para o GeoTools.
Para criar um novo módulo, é necessário seguir os seguintes passos:
	*Inicialmente é necessário mandar um e-mail aos responsáveis para adquirirem uma permissão para tal. 
	*De seguida é necessário criar um página no Wiki onde se irá colocar a documentação acerca do módulo que está a ser desenvolvido. 
	*E por fim assinar o Code Contribution License.
Assim que o módulo estiver numa versão estábel, pode ser submetido para a build partilhada. O que significa que, assim que o módulo for adicionado à build partilhada, quando alguém compilar o novo módulo que terá que compilar todo o projeto do GeoTools.
Idealmente deve-se trabalhar com alguém que possa confirmar que a build funciona com o setup do programador, e deve, se possível, testar com um repositório maven vazio, para garantir que outros utilizadores possam aceder a todas as dependências de que o novo módulo depende.
Quando o programador sentir que o seu módulo está pronto, pode decidir declará-lo formalmente supported, momento esse em que o módulo pode ser transferido para o directório modules/plugin/ ou modules/extension/.

