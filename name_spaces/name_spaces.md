### Moving Cells. 
#### Namespaces. 

THIS IS INITIAL DRAWT , PLEASE SEE 



In the drawing ..... we may see the hypothetical representation of human (or an animal) name space. It is done from the point of view of immune system cells, like lymphocytes. 

We think about our body as 2-D surface partitioned into unintersecting area. The Blood. This area is like a 'bus' in computer motherboard: all 'organs':  Lung, Skin, Liver.... are 'swimming' in the Blood and a lymphocite may 'swim' to any of organs from the Blood. 
We will use only Skin and Lung, it is enought for our purpases.  
We may see the 'handle' which is starting at an Organ at one side and attached to the Blood area at another side. The handle represent lymph collectors (on the Organ side) and lymph vessels coming back to the Blood veins on the other side. The lymph collectors are a garbige colectors filtrating our organs. In the middle of a handle we may see the Lymph Nodes: the place where immune cells interact between each other. The Nodes are a part of the filtration system. 

In this project we consentrate on the motion of the cells like our 'lymphocyte' in the name space environment with the untrivial topology: our partitioning is not a tree or a forest, but a cyclic graph. We may go from Blood to Skin, then to Lymph Collector, Lymph Node , Lymph Vessels and to Blood again by crossing each border between our areas only one time. 

The borders are very important part of our system. In our body a border is a collection of cells too. To come to an organ cell has to interact with border to get the permission to come  in. 

The cells of the borders are named in the way: 
B_L , where B is for Blood and L for Lung. $BL^+$ correspond to transition from Blood to Lung. $BL^-$ from Lung to Blood. 
It is possible to use $BL$  and $LB$ for the same purposes, but we would to use + and - as two possible orientations or the cyrcle boarders we use: left / right walks following the circle boarder. 

Vocabulary:  
BL the boarders between Blood and Lungs;  
BS : Blood and Skin;  
OC : between organs and Lymph Collector  
(we skip dependence from an  organ like SC or LC, it will be OC for all organs).
CN : Collector / Lymph Node
NV : Lymph Node / Lymph Vessel 
VB : Lymph Vessel / Blood

For the description of our system we will use the Milnor's pi-calculus. 

We will have the set of processes corresponding to the borders: 
$$Processes = SC^+|SC^-|BL^+|BS^-|BS^-|BS^+|OC^+|OC^-|CN^+|CN^-|CV^+|CV^-|VB^+|VB^-$$
We will describe a lymphocyte which demonstrate a 'homing': it permanently moves from Blood to Lungs, then to Lymph Collector, to Lymph Node, to Lymph Vessels and finally to Blood again. The agent is given by a recursive equation: 
$$Lymphocyte = \overline{BL^+}.\overline{OC^+}.\overline{CN^⁺}.\overline{NV^+}.\overline{VB^+}.Lymphocyte$$



$$|d_i>$$

$$Lymhocyte = \overline{L^+}.S^+.Lymphocyte$$

$$OurSystem = L$$

$$\bar{ə}$$
