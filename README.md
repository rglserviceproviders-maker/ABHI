#include <iostream>
#include <string>
using namespace std;

void showMenu() {
    cout << "=====================================\n";
    cout << "   Welcome to RGL Travels Website    \n";
    cout << "=====================================\n";
    cout << "Please choose a package/service:\n";
    cout << "1. Agra Sightseeing\n";
    cout << "2. Mathura Sightseeing\n";
    cout << "3. Airport & Station Drop Service\n";
    cout << "4. Outstation Cab Service\n";
    cout << "5. Exit\n";
    cout << "=====================================\n";
}

void showDetails(int choice) {
    switch(choice) {
        case 1:
            cout << "\nAgra Sightseeing Package:\n";
            cout << "- Visit Taj Mahal, Agra Fort, Mehtab Bagh\n";
            cout << "- Comfortable cab with professional driver\n";
            cout << "- Contact: 9012380804 / 9319341447\n";
            break;
        case 2:
            cout << "\nMathura Sightseeing Package:\n";
            cout << "- Visit Krishna Janmabhoomi, Dwarkadhish Temple\n";
            cout << "- Safe and clean cab service\n";
            cout << "- Contact: 9012380804 / 9319341447\n";
            break;
        case 3:
            cout << "\nAirport & Station Drop Service:\n";
            cout << "- Pick-up and drop from Delhi/Jaipur airports\n";
            cout << "- Railway station transfers available\n";
            cout << "- Contact: 9012380804 / 9319341447\n";
            break;
        case 4:
            cout << "\nOutstation Cab Service:\n";
            cout << "- Travel to Delhi, Jaipur, Fatehpur Sikri, etc.\n";
            cout << "- Affordable rates, timely service\n";
            cout << "- Contact: 9012380804 / 9319341447\n";
            break;
        case 5:
            cout << "\nThank you for visiting RGL Travels!\n";
            break;
        default:
            cout << "\nInvalid choice. Please try again.\n";
    }
}

int main() {
    int choice;
    do {
        showMenu();
        cout << "Enter your choice: ";
        cin >> choice;
        showDetails(choice);
        cout << "\n\n";
    } while(choice != 5);

    return 0;
}
