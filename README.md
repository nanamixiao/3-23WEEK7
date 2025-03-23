# 3-23WEEK7

## 
``` cpp

#include <iostream>

using namespace std;
struct Node{

    int theData;
    Node *nextNode;

    Node(int data = 0) : theData(data), nextNode(nullptr) {}
};



class LinkC{

    public: LinkC(){

    head = new Node();
    }



public :
    void  inserF(int val){
        Node* node = new Node(val);

        node->nextNode = head->nextNode;
        head->nextNode = node;


    }


public:
    void deletF(){

    
    Node* nodeVal = head->nextNode;
    head->nextNode = nodeVal->nextNode;



    delete nodeVal;

}



private: Node* head;




};
int main() {


}

```

## video
https://youtu.be/o_EW6atpy24
