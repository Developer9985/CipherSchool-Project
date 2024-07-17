# CipherSchool-Project
Binary Search Tree (BST) Project
This project implements a Binary Search Tree (BST) in C++. The BST supports various operations such as insertion, deletion, search, and traversal. The code also includes a menu-driven interface to interact with the BST.

Table of Contents
Binary Search Tree (BST) Project
Table of Contents
Node Structure
Functions
Insert
Insert Multiple
Search
Inorder Traversal
Preorder Traversal
Postorder Traversal
Delete Node
Print Tree
Display Menu
Main Function
Usage
Example
License

Node Structure
struct Node {
    int key;
    Node* left;
    Node* right;

    // Constructor
    Node(int k) : key(k), left(nullptr), right(nullptr) {}
};

A Node structure represents a node in the BST. Each node contains an integer key, a pointer to the left child, and a pointer to the right child. The constructor initializes the node with a given key and sets the left and right pointers to nullptr.

Functions
Insert
Node* insert(Node* root, int key);

Inserts a node with the given key into the BST. If the root is nullptr, it creates a new node with the key. If the key is less than the root's key, it inserts the key into the left subtree. If the key is greater than the root's key, it inserts the key into the right subtree.

Insert Multiple

Node* insertMultiple(Node* root, vector<int>& keys);

Inserts multiple keys into the BST. It iterates over the keys vector and calls the insert function for each key.

Search
bool search(Node* root, int key);
Searches for a node with the given key in the BST. If the key is found, it returns true. Otherwise, it returns false.

Inorder Traversal
void inorder(Node* root);
Performs an inorder traversal of the BST. It visits the left subtree, the root, and then the right subtree. The keys are printed in ascending order.

Preorder Traversal
void preorder(Node* root);
Performs a preorder traversal of the BST. It visits the root, the left subtree, and then the right subtree. The keys are printed in the order they are visited.

Postorder Traversal
void postorder(Node* root);
Performs a postorder traversal of the BST. It visits the left subtree, the right subtree, and then the root. The keys are printed in the order they are visited.

Delete Node
Node* deleteNode(Node* root, int key);
Deletes a node with the given key from the BST. If the node to be deleted has no children, it simply deletes the node. If the node has one child, it replaces the node with its child. If the node has two children, it replaces the node with its in-order successor (the smallest node in the right subtree) and deletes the in-order successor.

Print Tree
void printTree(Node* root, int space = 0, int indent = 5);

Prints the structure of the BST in a visually appealing way. It recursively prints the right subtree, the root, and then the left subtree with indentation to show the structure.

Display Menu
void displayMenu();
Displays a menu with options to insert a key, insert multiple keys, perform inorder, preorder, or postorder traversal, delete a key, print the tree structure, or exit the program.

Main Function
int main();

The main function initializes the BST root and provides a menu-driven interface to interact with the BST. It allows the user to choose different operations and perform them on the BST.

Usage
1.Insert Key: Insert a single key into the BST.
2.Insert Multiple Keys: Insert multiple keys into the BST.
3.Inorder Traversal: Perform an inorder traversal of the BST.
4.Preorder Traversal: Perform a preorder traversal of the BST.
5.Postorder Traversal: Perform a postorder traversal of the BST.
6.Delete Key: Delete a node with a specific key from the BST.
7.Print Tree: Print the structure of the BST.
8.Exit: Exit the program.
