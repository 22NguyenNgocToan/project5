#include <bits/stdc++.h>
using namespace std;

string getSnippet(int choice) {
    switch(choice) {
        case 1: return "for (int i = 0; i < n; ++i) {\n    // code here\n}";
        case 2: return "if (condition) {\n    // code\n} else {\n    // code\n}";
        case 3: return "struct Student {\n    string name;\n    int age;\n};";
        case 4: return "class Calculator {\npublic:\n    int add(int a, int b) { return a + b; }\n};";
        default: return "// Lựa chọn không hợp lệ!";
    }
}

int main() {
    cout << "=== Code Snippet Generator 🧠 ===\n";
    cout << "1. For Loop\n2. If-Else\n3. Struct\n4. Class\n";
    cout << "Chọn loại snippet: ";
    int n; cin >> n;
    cout << "\nKết quả:\n" << getSnippet(n);
}
