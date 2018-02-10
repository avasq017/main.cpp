#include <iostream>
using namespace std;
main () {
    string word;
    getline (cin, word);
    for (int i = 0; i < word.length(); ++i) {
        if(word.at(i) == ' ') {
            word.erase(i,1);
            --i;
        }
    }
    cout << word << endl;
    return 0;
}
