# Cloning laravel project from GitHub
---> .env will not be cloned; .env.example will be uploaded; copy paste everything; command- php artisan key:generate

#Login Laravel
---> $credentials = $request->only('email', 'password'); if (Auth::attempt($credentials)){
            return redirect()->route('admin')->with('success', 'Login Successfull!');
        } else {
            return redirect()->back()->with('error', "Please Enter Correct Email and Password");
        }
---> register and login will have POST method
---> always save data in built in User() database
