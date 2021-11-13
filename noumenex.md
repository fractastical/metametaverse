# Noumenex
## Metaverse language

### Rationale: Language as an optimization function

Process optimization for bridging experience between two nodes (e.g. persons) including the direct passing of a complex phenomenon that cannot easily be expressed in a word.

Problem: I want to express an idea like "the cat is on the table"

Solution: I use my mouth to utter the words "the cat is on the table." Other person hears the phrase and understands that the cat is on the table.

Solution map:  `(node1((idea (noun(location)) -> (mouth(phrase))) -> (node2(ear(brain-interpreter)) -> (idea (noun(location)))`
Additional context: both parties (node1 and node2) must have already seen "the cat" and have a mental model of what that describes. 

For the solution map we can optimize for two functions, fidelity and speed. Fidelity is defined as the extent to which the object (in this case (noun(location) ) is the same in the original node (mind of person 1) and in the second node (mind of person 2). In this case, various testing functions are possible. For example, asking the question to both parties: Where is the cat?  What is on the table? This forces the knowledge transfer function to an effectively binary conclusion.  

Speed is the time it takes to finish the process. In this case, a matter of seconds, probably under 10 seconds. However, this can always be optimized for.

Now the problem is that with more complex ideas (more strictly "noumena") both of these functions are harder to express. The testing function is harder to bring to a binary ouput and the time to express increases. 

Problem: I want to express an idea like "the dodecahedron is inside the third metaverse on the left"

Solution: I create Rendering through a set of objects and rendering engines, I load them into virtual reality glasses. I give them to other person. They put on the glasses and observe. 

Solution map:  `(node1((idea (noun(location)) -> (rendering engine(object))) -> (node2(vr-goggles(eyes(brain-interpreter)) -> (idea (noun(location)))`

In the first example we used standard motor functions and sensory organs with the middleware layer of soundwaves which both our vocal organs and auditory organs are preconfigured for. In this second example we have a more complex middleware layer that consists of a mix of proprietary hardware and software which has a similar function, namely transmitting complex data forms into a visually accessible format. 

As with our two optimization parameters from the first example, fidelity and speed, we are now in the place where we can make reliable comparisons between different media types and comparison mechanisms. Moreover, these can be optimized for. 

Consequently, a capital deployment and product delivery cycle can be designed that consists of the optimization for these variables. 

### Additional challenges 

Many topical matters (abstract geometries, synesthesic poetic experiences, pheromones, dreams) do not immediately or easily lend themselves to direct communication with other parties. That said, our language is perhaps the first to make them accessible. Additionally, while with an emphasis on the visual, it is by no means exclusively limited to such, and the relative increase in availablity of certain technologies (i.e. AR/VR/MR) allows the data transfer rate to rapidly increase with more complex and synesthesic experiences. This means that "noumenex" as a language is potentially the ultimate dense and meaningful expressiveness yet known to humanity.  


### Nouns in this language

Reference has already been made to location. Location can be releative (with reference to a known object) or absolute, with respect to a known coordinate system. In metaverses, an effort has been made to provide a universal nomenclature that can be used for all locations in all metaverses. The way we do this is as follows, starting with the meta metaverse each location can be described as a vector (x,y,z) from the central point (0,0,0). 

If each point can also be a portal which includes a transform, including of the rendering engine, then each vector (or set of vectors) can resolve to a specific point in another metaverse. 

`(1,2,3) -> (metaverse2.url(renderingEngine))`

In order to explore, this does require that the client be able to load multiple rendering engines in order to go from one metaverse to the next. 

This effectively makes Noumenex a universal language for traversing all metaverses. 

### Verbs in this language


#### GO
 

`-> (1,2,3)` 

Go to coordinates (1,2,3) 

 
#### Zoom


One key type of action specific the meta metaverse is "zoom"

`-> (1,2,3) -> (zoom(2)) -> (3,2,3) `

Go to  (1,2,3) then zoom 2 scale factors then go +3 in the x coordinates, +2 in the y coordinates, and +3 in the z coordinates 


#### Insert

`-> (1,2,3) -> (insert(house.xtz240.ipfs.org)) `

Insert a house at the coordinates (1,2,3) 


#### Rotate (not sure this is necessary) 

Rotating refers to the users view orientation  

`-> (1,2,3) -> Rotate(20d,-20d) `


### Access Control


`-> (1,2,3) -> (access(insert(house.xtz240.ipfs.org)),guildDAO(edit))`

Move cursor to 1,2,3. Insert a house, Give guildDAO members access to edit the space. 

Practically speaking this will need to be included as an addition to a token specification  

`getAccessControl(type.edit)`


### Standard ERC721 functions from OpenZepplin


### Additional necessary functions

`function getLocation() public view virtual override returns (string[])`
   
Get location as a set of vectors 

`function getEditAccess() public view virtual override returns (addresses[])`

Get location as a set of ethereum address (including DAOs) that have edit access

`function hasAccess(address) public view virtual override returns (bool)`

Returns if the given address has access rights or not 



### Standard ERC721 functions that must also be supported 




`contract ERC721 is Context, ERC165, IERC721,IERC721Metadata {
  
  
    constructor(string memory name_, string memory symbol_) 
    function supportsInterface(bytes4 interfaceId) public view virtual override(ERC165, IERC165) returns (bool) 
    function balanceOf(address owner) public view virtual override returns (uint256)
    function ownerOf(uint256 tokenId) public view virtual override returns (address) 
    function name() public view virtual override returns (string memory) 
    function symbol() public view virtual override returns (string memory) 
    function tokenURI(uint256 tokenId) p
    function approve(address to, uint256 tokenId) public virtual override
    function getApproved(uint256 tokenId) public view virtual override returns (address) 
    function setApprovalForAll(address operator, bool approved) public virtual override
    function isApprovedForAll(address owner, address operator) public view virtual override returns (bool) {
        return _operatorApprovals[owner][operator];
    function transferFrom(
        address from,
        address to,
        uint256 tokenId
    ) public virtual override

    function safeTransferFrom(
        address from,
        address to,
        uint256 tokenId
    ) 

    function safeTransferFrom(
        address from,
        address to,
        uint256 tokenId,
        bytes memory _data
    ) 

    function _safeTransfer(
        address from,
        address to,
        uint256 tokenId,
        bytes memory _data
    ) internal virtual 

    function _exists(uint256 tokenId) internal view virtual returns (bool) 


    function _isApprovedOrOwner(address spender, uint256 tokenId) internal view virtual returns (bool) 


    function _safeMint(
        address to,
        uint256 tokenId,
        bytes memory _data
    ) internal virtual {

    function _mint(address to, uint256 tokenId) internal virtual 


    function _burn(uint256 tokenId) internal virtual


    function _transfer(
        address from,
        address to,
        uint256 tokenId
    ) internal virtual 

    function _approve(address to, uint256 tokenId) internal virtual {
        _tokenApprovals[tokenId] = to;
        emit Approval(ERC721.ownerOf(tokenId), to, tokenId);
    }

    function _setApprovalForAll(
        address owner,
        address operator,
        bool approved
    ) internal virtual


    function _checkOnERC721Received(
        address from,
        address to,
        uint256 tokenId,
        bytes memory _data
    ) 
    
    
    function _beforeTokenTransfer(
        address from,
        address to,
        uint256 tokenId
    ) internal virtual {}
    
    





TOADD: Metadata encompassing ms for data transfer per step, fidelity, testing formulas, testing framework, graphics of user interfaces. 


