# link-listt
#include <iostream>

using namespace std;

class Node{
    public:
    int data;
        Node * next;
};

void print_list(Node*n)
{
    cout << "print list of node"<<endl;
    while(n!=NULL){
        cout <<n->data<<endl;
        n=n->next;
    }
}

int main()
{
    cout<<"link list"<<endl;
    Node * head;
   Node * second;
   
    head = new Node();
    second = new Node();
    
    head->data=12;
    head->next = second;
    
    head->data=13;
  second->next = NULL;
  
    
 //cout<< "head data"<<head->data<<endl;
  //cout<< "head data"<<head->data<<endl;
   print_list(head);
  return 0;
  
   
}
