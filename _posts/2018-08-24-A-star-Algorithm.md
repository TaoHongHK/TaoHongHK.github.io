---
layout: post
title: A* Algorithm
date: 2018-08-24 20:28:20 +0300
description: my Algorithm . # Add post description (optional)
img: post-1.jpg # Add image post (optional)
tags: [Algorithm, Java]

---

# **A*�㷨**


---

## **���**

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-88d440f686f78ef7.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/800">
</center>


һֻѰ·��è

�����ǿ�ʼ����������һ����������Ϸ��һֻè��Ҫ�ҵ�һ��ͨ��һ����ͷ��·��

��ô��������������������ͼƬ���è��Ҫ�ҵ�ͨ����ͷ�����·����

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-6d0b5383f850aa24.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

���˱��˵��ǣ�è�䲻��ֱ�Ӵ���Ŀǰ��λ���ߵ���ͷ���ڵ�λ�ã���Ϊ��һ��ǽ��ס��·����������Ϸ��Ҳ����һ����ʵ��Ĺ�꣡������Ϸ�����ֻèҲ������������һ����˵��Ҫ�ҵ�һ����̵�·��.��ô����������ô����д��һ���㷨ȥ�ҵ�è��Ӧ���ߵ����·���أ� A* ���ǽ�ȷ�����

����������򵥻�

��Ѱ·�����У�����Ҫ���ĵ�һ�����ǽ����������ΪһЩ�����ܹ������׹���Ķ�����������ôȥ�����ȡ���������Ϸ�����磺���ǿ��Խ���������ָ���һ��һ�������أ�������������������ֻ��ڴ�ש��tile������Ϸ��˵�����������λ̫С�ˡ����ԣ����ǽ��ô�ש�������Σ���Ϊ������λ��Ѱ·�㷨��ʹ�á�������״��Ҳ���ԣ����������λ������Σ��������������������������Ҫ�ģ�����Ҳ����򵥵ġ�
�������ָ����������ǵ���������Ϳ��Ա��򵥵ı�ʾΪһ����ά���顣���Ե����ǵĹؿ��� 25x25 �Ĵ�שʱ�����ǵ������������һ������625�������ε����顣������ǽ����ǵĵ�ͼ�����طָ�����ʱ�����ǵ���������ͽ�����һ������ 6400,000 �������ε����飨һ����ש�� 32x32 �����أ���

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-778f0baa19155925.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

���ű�ͱպϱ�
���������Ѿ�����һ���򵥵��������������������� A* �㷨 ����ôʵ�ֵġ�
���ǵ�è��������裬����Ҳ���ã�����������Ҫ������
һ�������ڼ�¼�������ڱ����ǡ������ҵ����·���ķ������ǽ������ű�
һ�������ڼ�¼���в���Ҫ���ٴο��ǵķ������ǽ����պϱ�
�տ�ʼʱ��è�佫��Ŀǰ��λ�ã����ǽ��ƺ������ʼ�ĵ�Ϊ�㡰A��������պϱ��С�Ȼ�����������ڽ����ġ��������ߵķ�����뿪�ű��С�
�����һ������չʾ�����è��վ��һ������λ�ã�Ӧ����ô������ɫ�����ű�

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-f78b4169a0b80fe6.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

·������
���ǽ���ÿһ������һ��������G + H
G�����Ŵӿ�ʼ�㡰A����Ŀǰ���ڷ���Ĵ��ۡ����ԣ�����һ���ڽ���ʼ�㡰A���ĵ���˵�����۾���1, ���ǵ������뿪ʼ��ԽԶʱ�����۾ͻ����ӡ�
H�����Ŵӵ�ǰ�㵽Ŀ�ĵص��Ԥ�ƴ��ۣ����ǽ��ѹ�ͷ���ڵĵ��Ϊ�㡰B�������������ͨ���ǳ����Եļ���ó��� �C ��Ϊ���ǲ�֪�������Ĵ����Ƕ��٣��������һ�����ơ�
����ܻ��룬���ƶ����ۡ��ĺ�����ʲô����ʵ����Ϸ������൱�� �C ����ֻ�Ƿ�����������ˡ�
Ȼ������ס�����ǵ���Ϸ�У�����Ը�������ͬ�ĺ��塣���磺
���������Խ����ƶ��Ļ�������ܻὫ�Խ����ƶ��Ĵ������õ��Ը�һ�㡣
������м��ֲ�ͬ�ĵ��Σ�����ܻ����ò�ͬ���ƶ������ڲ�ͬ�ĵ����ϡ�
����Ǵ��µ��뷨 �C ����������������������ļ��� G �� H �ɡ�

���� G
Ϊ�˼��� G��������Ҫ����һ�� G �����������Ǹ������ټ���1����ˣ�ÿһ������� G ֵ������� A ����·�������������ܴ��ۡ�
���磬�����ͼ��չʾ����������ͬ��ͷ��·����ÿһ������� G ֵ���Ѿ������ȥ�ˡ�

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-5c620ec59ca2ffff.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

���� H
����һ�£�H �Ǵӵ�ǰ����Ŀ�ĵص�Ԥ�ƻ��ѡ�
Ԥ�ƻ���Խ�ӽ�ʵ�ʴ��ۣ����յ�·���ͻ�Խ׼ȷ�����Ԥ�Ƶò���׼ȷ����ô���ɵ�·�����ܲ�����̵ģ����������ܻ�ܽӽ������������̫���ڸ������������ǽ���������ƪ�̳����������������һ��ǻ�������ĩβ������һ���������͵�ʮ���꾡�����ӡ�
Ϊ�˽����򵥻������ǽ����õ��������˾����㷨������ע��Manhattan distance method��������㷨����ֻ�Ǽ����˵�ǰ�㵽 B ���ˮƽ�������ֱ�����ϵķ���������û�н��ϰ����ͬ���ο��ǽ�����
���磬������ͼ��չʾ���ڲ�ͬ��ʼ���£��á������˾����㷨��ģ��� H ֵ����ʾ�ںڿ��У�

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-0d82daa7ed0b4b47.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

A* �㷨
��ô������֪�������ȥ����ÿһ������ķ��������ǽ���������� F�������� G + H��
è����ظ�һ�²������ҵ����·����
�ڿ��ű����õ�һ��������͵ķ������ǽ��������������� S
�ڿ��ű����Ƴ����� S��Ȼ�� S ����պϱ���
�����ڷ��� S ��ÿһ�����ڵķ��� T
A. ��� T �ڱպϱ��У�������
B. ��� T ���ڿ��ű��У��������뿪�ű��У�Ȼ��������Ĵ���
C. ��� T �Ѿ��ڿ��ű��У������������õ�ǰ���ɵ�·�������յ�Ļ���F ֵ�᲻����͡�����ǵĻ�����ô����������ֵ��Ȼ��Ҳ�������ĸ��ڵ�
������������̫�˽�Ļ������� �C ���ǽ�ͨ��һ���򵥵�������һ��һ������ʾ�������������ģ� :)
è���·��
��������һ����è����ҵ���ͷ����Ϊ���ӡ�
������ı���У����Ѿ��������µķ�ʽ�г��� F = G + H ��ֵ:
F��ÿ���������ֵ���� �����Ͻ�
G���� A ����ǰ����Ĵ��ۣ��� ���½�
H���ӵ�ǰ���� B ���Ԥ�����ۣ��� ���½�
����֮�⣬��ͷ��ʾ�˵���÷�����ƶ�����
���ÿһ���ĺ�ɫ�������պϱ���ɫ��������ű�
�ã������ǿ�ʼ�ɣ�
Step 1
�ڵ�һ����è��ȷ������������ʼ�㣨�� A�����ڵĿ����ߵķ��񣬼������ǵ� F ֵ��Ȼ�����Ǽ������Ŀ��ű��С�

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-e2b45fffeafe57d8.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

��ᷢ��ÿ������� H ֵ���Ѿ��г����ˣ�����������6��һ����4�����ҽ������� ������������㷨��������ÿһ������� H ֵ���Ա�������⡣
ͬ����Ҫ���ѵģ�F ֵ�������Ͻǣ��ͽ����� G+H ��ֵ��
Step 2
����һ����è��ѡ���� F ֵ��͵ķ��񣬽�������պϱ��У�Ȼ����������ڽ�����

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-9dbd682fca87c00c.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

���������ܿ�����������͵ķ����� F ֵΪ 5 �ķ��������Խ����е����ڷ�����뿪�ű��У�Ȼ��������ǵ���ֵ����Ҫע�⵽�����ܽ�è�����ڵķ�����뿪�ű���Ϊ���Ѿ��ڱպϱ����ˣ�����Щ�ϰ��﷽��Ҳ���ܼ��루��Ϊ���ǲ������ߵģ���
��Ҫע����ǣ����������¼��뿪�ű�ķ������ǵ� G ֵ�Ѿ�����һ����Ϊ�������ʼ������������ľ��롣��ͬ��Ҳ��Ҫ�á�����������㷨����ȷ��ÿ���·���� H ֵ��
Step 3
ͬ���ģ�����ѡ����������� F ֵ�ķ��飬Ȼ�����������

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-7a5be4ef9bef56f0.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

Step 4
������������һ����Ȥ�����ӡ�����һ��ͼƬ������Կ����������� 4 ������������ͬ�� F ֵΪ 7 �� ��������Ӧ����ô����
���������м��ַ�ʽ�����ã�����һ���򵥵ģ�Ҳ�ǿ��ٵģ���ʽ�Ǽ����������һ�����뵽���ű��еķ����������Ǽ����������һ���ոռ�������ű��еķ���

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-01c73bab405785e4.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

��һ�����������ڵĶ��ҿ������ߵķ�����������ǰ�����������ǵķ�����
Step 5
������һ��������ѡ����������ͷֵķ���7��������Ϊ�˱���һ���������ѡ�������ڽ���һ������

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-52db9e68d28bb63f.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

��һ��ֻ��һ�ֿ����ԣ�����Խ��Խ�ӽ��ˣ�
Step 6
������Խ��Խ���ˣ��ҸҴ�ģ����²���һ���������ӵģ�

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-80c0605ef6d37a9d.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

���Ǽ�����Ҫ���ˣ�������Σ�����Կ�������������������������̵�·���ﵽĿ�ĵأ����ǿ�����������֮��ѡ��

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-13d93ccd69728a2b.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>


��������������У����������·����
1-2-3-4-5-6
1-2-3-4-5-7
�������Ĵ���ʵ���У�����ѡ������·������Ҫ��
Step 7
�������ٴε�����Щ����

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-d645efe5da27aba5.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

��������ͷ�����ڿ��ű��У�
Step 8
�����ǵ�Ŀ���ڿ��ű���ʱ���㷨�Ὣ�����뵽�պϱ��У�

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-3a95517b21d7dbb6.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

Ȼ���㷨������Ҫ���ľ��Ƿ���ȥ���ҵ����յ�·����

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-2ced77a8b199c504.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>

һ��û���۹��è�䣨A Non-Visionary Cat��
��������������У����ǿ��Կ�������è����Ѱ�����·��ʱ����ͨ����ѡ�����ŵķ���������δ�������·�����ϵķ��� �C ����������һ����������è�䣡����ע��ָ��Ӧ����̰�ĵ���˼��
���ǣ������ǵ�è�䣬û����ô��������������ѡ�񿪷ű��� F ��͵ķ���������ıպϱ����ô���أ�
��ͼչʾ��������Ѱ�����·���Ĺ���������Ҫ�����з�������Կ�����è�䳢���˸��෽�񣬵�������Ȼ�ҵ������·������֮ǰչʾ�Ĳ���һ���ģ�������һ����ȣ���

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-32112e106a0a67e9.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>


��ͼ�У���ɫ���񲢲��������·�������ǽ���ֻ�Ǳ�ʾ��������Щʱ��ѡΪ�� ��S�� ����
�ҽ����㿴������ı��Ȼ�����Լ�����������һ�Σ����ۺ�ʱ�㿴����һ������ƽ�ȵķ������ȥѡ��������ᷢ���������Ȼ�������·����β��
���ԣ���ᷢ�֣����� ������ �ķ�����Ҳû�����⣬����Ȼ�������·����β����ʹ�����ܻ������������Ρ�
���������ǵ�ʵ���У����ǽ��������㷨��������뵽���ű��У�
���ڷ��񽫻���������˳�򷵻أ���/��/��/��
һ�����񽫻ᱻ����뿪�ű��У�������������ͬ���۵ķ���֮�����Ե�һ�����뿪�ű��еķ��񽫻��ǵ�һ����è��ѡ��ķ���
������һ����ͼ��չʾ�Ļ��ݹ��̣�

<center class = "A*">
<img src="https://upload-images.jianshu.io/upload_images/13484241-29cbed722fe8e418.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240">
</center>


## **��������**

1. Coord������

```
public class Coord{
    public int x;
    public int y;
    
    public Coord(int x,int y){
        this.x = x;
        this.y = y;
    }
    
    @Override
    public boolean equals(Object obj){
        if(obj == null) return false;
        else if(obj instanceof Coord){
            Coord c = (Coord)obj;
            return x == c.x && y == c.y;
        }
        else return false;
    }
}
```

���ն�ά������ص㣬����ԭ�������Ͻǣ�����y�Ǹߣ�x�ǿ�y���µ�����x���ҵ��������ǽ�x��y��װ��һ���࣬������д��equals�����������Ƚ�������������Ƿ�����ͬ��

2.Node������

```
public class Node implements Comparabel<Node>{
     public Coord coord;
    public Node parent;
    public int G;
    public int H;

    public Node(int x,int y){
        this.coord = new Coord(x,y);
    }

    public Node(Coord coord,Node parent,int g,int h){
        this.coord = coord;
        this.parent = parent;
        G = g;
        H = h;
    }

    @Override
    public int compareTo(Node o){
        if(o == null) return -1;
        if(G + H > o.G+o.H){
            return 1;
        }
        else if(G + H < o.G + o.H) return -1;
        else return 0;
    }
}
```

��Node��̳�Comparabel�࣬�Ӷ�ʹ�����ȶ��е�ʱ����Խ�������������������

3.MapInfo������

```
public class MapInfo {
    public int[][] maps;
    public int width;
    public int height;
    public Node start;
    public Node end;

    public MapInfo(int[][] maps,int width,int height,
                   Node start,Node end){
        this.maps = maps;
        this.width = width;
        this.height = height;
        this.start = start;
        this.end = end;
    }
}
```

## **A_Star��**

```
public class A_Star {
    public final static int BAR = 1;
    public final static int PATH = 2;
    public final static int DIRECT_VALUE = 10;
    public final static int OBLIQUE_VALUE = 14;

    Queue<Node> openList = new PriorityQueue<Node>();
    List<Node> closeList = new ArrayList<Node>();

    public void start(MapInfo mapInfo){
        if(mapInfo == null) return;
        openList.clear();
        closeList.clear();
        openList.add(mapInfo.start);
        moveNodes(mapInfo);
    }

    private void moveNodes(MapInfo mapInfo){
        while(!openList.isEmpty()){
            if(isCoordInClose(mapInfo.end.coord)){
                drawPath(mapInfo.maps,mapInfo.end);
                break;
            }
            Node current = openList.poll();
            closeList.add(current);
            addNeighborNodeInOpen(mapInfo,current);
        }
    }

    private boolean isCoordInClose(Coord coord){
        if(closeList.isEmpty()) return false;
        for(Node node: closeList){
            if(node.coord.equals(coord)){
                return true;
            }
        }
        return false;
    }

    private Node findNodeInOpen(Coord coord){
        if(coord == null || openList.isEmpty()) return null;
        for(Node node : openList){
            if(node.coord.equals(coord)){
                return node;
            }
        }
        return null;
    }

    private boolean isEndNode(Coord end,Coord coord){
        return coord!=null && end.equals(coord);
    }

    private int calcH(Coord end,Coord coord){
        return (Math.abs(end.x - coord.x)+ Math.abs(end.y -coord.y))*10;
    }

    private boolean canAddNodeToOpen(MapInfo mapInfo,int x,int y){
        if(x<0||x>=mapInfo.width||y<0||y>=mapInfo.height)
            return false;
        else if(mapInfo.maps[y][x] == BAR) return false;
        else if(isCoordInClose(x,y)) return false;
        else return true;
    }

    private void addNeighborNodeInOpen(MapInfo mapInfo,Node current
    ,int x,int y,int value){
        Coord coord = new Coord(x,y);
        if(canAddNodeToOpen(mapInfo,x,y)){
            Node end = mapInfo.end;
            int G = current.G + value;
            Node child = findNodeInOpen(coord);
            if(child == null){
                int H = calcH(end.coord,coord);
                if(isEndNode(end.coord,coord)){
                    child = end;
                    child.parent = current;
                    child.G = G;
                    child.H = H;
                }
                else child = new Node(coord,current,G,H);
            }
            else if(child.G>G){
                child.G = G;
                child.parent = current;
            }
            openList.add(child);
        }
    }

    private void addNeighborNodeInOpen(MapInfo mapInfo,Node current){
        int x = current.coord.x;
        int y = current.coord.y;
        addNeighborNodeInOpen(mapInfo, current,x-1,y,DIRECT_VALUE);
        addNeighborNodeInOpen(mapInfo, current,x,y-1,DIRECT_VALUE);
        addNeighborNodeInOpen(mapInfo, current,x+1,y,DIRECT_VALUE);
        addNeighborNodeInOpen(mapInfo, current,x,y+1,DIRECT_VALUE);
        addNeighborNodeInOpen(mapInfo, current,x-1,y-1,OBLIQUE_VALUE);
        addNeighborNodeInOpen(mapInfo, current,x+1,y-1,OBLIQUE_VALUE);
        addNeighborNodeInOpen(mapInfo, current,x-1,y+1,OBLIQUE_VALUE);
        addNeighborNodeInOpen(mapInfo, current,x+1,y+1,OBLIQUE_VALUE);

    }

    private void drawPath(int[][] maps,Node end){
        if(end == null || maps == null) return;
        System.out.println("totalValue: "+end.G);
        while(end!=null){
            Coord c = end.coord;
            maps[c.y][c.x] = PATH;
            end = end.parent;
        }
    }
    
    public static void printMap(int[][] maps){
        for(int i = 0;i<maps.length;i++){
            for(int j = 0;j<maps[i].length;j++){
                System.out.print(maps[i][j]+" ");
            }
            System.out.println();
        }
    }
    
    public static boolean inputRight(MapInfo mapinfo){
        Coord end = mapinfo.end.coord;
        Coord start = mapinfo.start
        return !(mapinfo.maps[end.y][end.x]==BAR||mapinfo.maps[start.y][start.x]);
    }
}

```

## **text**

```

public class Text{
    public static void main(String[] args) {
                int[][] maps = {
                {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1},
                {1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1},
                {1, 0, 1, 0, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1},
                {1, 0, 1, 0, 1, 0, 1, 0, 0, 1, 1, 1, 1, 1, 0, 1},
                {1, 0, 1, 0, 1, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1},
                {1, 0, 0, 1, 1, 0, 1, 1, 0, 0, 0, 0, 0, 0, 0, 1},
                {1, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1},
                {1, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 1},
                {1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1}
        };
        A_Star a_star = new A_Star();
        MapInfo mapinfo = new MapInfo(maps, maps[0].length, maps.length,
                new Node(3, 4), new Node(12, 5));
        if (a_star.inputRight(mapinfo)) {
            a_star.start(mapinfo);
            A_Star.printMap(maps);
        } else System.err.println("Input Wrong");
    }
    }
}

```


