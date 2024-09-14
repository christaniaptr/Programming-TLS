temperature;
    string temptFrom, temptTo;
    
    
    cout << "Please enter the temperature unit you want to convert from (Celcius, Fahrenheit, Kelvin): " ;
    cin >> temptFrom;
    
    
    cout << "What temperature unit do you want to convert it to? (Celcius, Fahrenheit, Kelvin): " ;
    cin >> temptTo;
    
    cout << "Enter the temperature you want to convert : ";
    cin >> temperature;
    
    if (temptFrom == "Celcius" || temptFrom == "celcius") {
        if (temptTo == "Fahrenheit" || temptTo == "fahrenheit") {
            double fahrenheit = (temperature*9/5)+32;
            cout << "Your result is " << fahrenheit << "degrees Fahrenheit" << endl;
        } else if (temptTo == "Kelvin" ||temptTo == "kelvin") {
            double kelvin = temperature+273;
            cout << "Your result is " << kelvin << "degrees Kelvin" << endl;
        }
    } else if (temptFrom == "Fahrenheit" || temptFrom == "fahrenheit") {
        if (temptTo == "Celcius" || temptTo == "celcius" ) {
            double celcius = (temperature-32)*5/9;
            cout << "Your result is " << celcius << "degrees Celcius" << endl;
        } else if (temptTo == "Kelvin" || temptTo == "kelvin") {
            double kelvin = (temperature-32)*5/9+273;
            cout << "Your result is " << kelvin << "degrees Kelvin" << endl;
        }
    } else if (temptFrom == "Kelvin" || temptFrom == "kelvin") {
        if (temptTo == "Celcius" || temptTo == "celcius") {
            double celcius = temperature-273;
            cout << "Your result is " << celcius << " degrees Celcius" << endl;
        } else if (temptTo == "Fahrenheit" || temptTo == "fahrenheit") {
            double fahrenheit = (temperature-273)*9/5+32;
            cout << "Your result is " << fahrenheit << "degrees Fahrenheit" << endl;
        }
        return 0;
    }
    }
