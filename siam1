#include<bits/stdc++.h>
using namespace std;

class node
{
public:

    int data;

    node* nxt;

    node* prev;

};

class doublelink
{
public:

    node* head;
    int sz=0;

    doublelink()
    {
        head=NULL;
    }

    node* create(int val)
    {
        node* a=new node;

        a->data=val;
        a->nxt=NULL;
        a->prev=NULL;

        return a;



    }

    void push(int val)
    {
        sz++;
        node* a=create(val);

        if(head==NULL)
        {
            head=a;
            return;
        }

        node* b=head;

        b->prev=a;
        a->nxt=b;
        head=a;
    }

    void pop()
    {

        if(head==NULL)
        {
            return;
        }

        node* b=head;

        head=b->nxt;

        delete b;
        sz--;

    }

    int getsize()
    {
        return sz;
    }

    int top()
    {

        return head->data;
    }

    void allelements()
    {
        node*a=head;

        while(a!=NULL)
        {
            cout<<a->data<<endl;

            a=a->nxt;



        }
    }



};

int main()
{
    doublelink st;
    doublelink temp;

    st.push(5);
    st.push(6);
    st.push(7);

    while(st.getsize()>0)
    {
        temp.push(st.top());

        st.pop();
    }

//    cout<<st.getsize();
//    cout<<endl;
//    st.top();
//
//    st.pop();
//
//    cout<<"After pop "
//            <<endl;


    //cout<<endl;

    swap(st,temp);


    st.allelements();


}
