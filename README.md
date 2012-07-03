SlimeRefresh
=================================================

A lovely refresh style looks like ``` UIRefreshControl ```. It's looks like the Slime so I name it SlimeRefresh.

Screenshot:

![screenshots](http://zhaorenzhi.cn/wp-content/uploads/2012/06/687474703a2f2f7777772e73637461622e636f6d3a383038302f6674702f73637265656e73686f74312e706e67.png)

How to use?
==================================================

1,down the source from https://github.com/dbsGen/SlimeRefresh/

2,add all under SlimeRefresh/SlimeRefresh to your project.

3,#import "SRRefreshView.h"

4,init SRRefreshView and add it to a UIScrollView.

Protocol 
==================================================

    - (void)slimeRefreshStartRefresh:(SRRefreshView*)refreshView;
    
Only one protocol, you have to implement. it will be called when the refreshing will be executed.

Style
==================================================

- Change to style of the slime, You have to get the instance of SRSlimeView by this ```    refreshView.slime    ```
  - ``` viscous ``` this property to set how the limit of the slime being pulled apart.
  - ``` radius ``` to set the size of slime.
  - ``` bodyColor ``` to set the fill color.
  - ``` skinColor ``` to set the line color.

- How to set the arrow image?
  - ``` refreshView.refleshView.image ``` use this to set the arrow image.

Up inset
==================================================

Some time you maybe want to add the ``` SRRefreshView ``` to a ``` UIScrollView ``` which 

have setted the ``` contentInset ```. At this time you will set the ``` upInset ``` 