import math
def minMaxAlgo(currNode,nodeindex,maxturn,leafnodes,nodedepth):
    if(currNode==nodedepth):
        return leafnodes[nodeindex]
    if(maxturn):
        return max(minMaxAlgo(currNode+1,nodeindex*2,False,leafnodes,nodedepth),
              minMaxAlgo(currNode+1,nodeindex*2+1,False,leafnodes,nodedepth))

    else:
        return min(minMaxAlgo(currNode+1,nodeindex*2,True,leafnodes,nodedepth),
              minMaxAlgo(currNode+1,nodeindex*2+1,True,leafnodes,nodedepth))

        

leafnodes=[2,4,6,4,2,4,6,4]
nodedepth=math.log(len(leafnodes),2)
minMaxAlgo(0,0,True,leafnodes,nodedepth)
