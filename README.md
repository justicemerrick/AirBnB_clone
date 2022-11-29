<h1>AirBnB Clone Project</h1>
    <h2>Project Description</h2>
    <p>
      This is the Part I of the AirBnB project. We worked on the backend of the project,
       using the console as an interface with the help of python's cmd module. <br> <br>The python objects(data) 
       generated were stored in a json file which is to be accessed wth the help of
       python's jason module.
    </p>
    
 <h2>Description of the command interpreter</h2>
 <p>
  The interface of the project is synonymous to a bash shell.
  However, the difference is in it's limited number of commands
  which were exclusively defined for this project - The AirBnB website clone. <br><br>
  Therefore, we would refer the command line interpreter as the frontend of this project.
  This is the medium through which users can interact with the backend which we
  developed using Python's OOP.
</P>


<p><b> Here are the available commands in this project</b></p>

<ul>
  <li><em>Show</em></li>
  <li><em>Create</em></li>
  <li><em>Update</em></li>
  <li><em>Destroy</em></li>
  <li><em>Count</em></li>
</ul>

<p><b>With regards to the command line usage, in relation to the backend and the storage system,
      The following actions can be executed:</b></p>
  <ul>
      <li><em>Creating new objects (ex: a new User or a new Place)</em></li>
      <li><em>Retrieving an object from a file, a database etc…</em></li>
      <li><em>Doing operations on objects (count, compute stats, etc…)</em></li>
      <li><em>Updating attributes of an object</em></li>
      <li><em>Destroying an object</em></li> 
  </ul>
  
  <H2>How to start it</H2>
  <p>The following instructions will get you a copy of 
     the project up and running on your local machine (Linux distro)
     exclusively for development and testing purposes.</p>
     
  <H2>Installing</H2>
  <p>To install this program, there is the need to clone the repository from github <br> includes the shell program and associated dependencies.
            You will need to clone the repository of the project from Github. This will contain the simple shell program and all of
            its dependencies. Below are simple steps you can follow to install the program:</p>
 
            git clone https://github.com/justicemerrick/AirBnB_clone.git
            
            
<p>Once the cloning is done, you will have a folder containing the the AirBnB project. In this folder, you're expected to see
                several files with which the program can run. They include:</p>
   
   <ul>
                    <li><em>/console.py </em>: The main executable of the project, the command interpreter.</li>
                    <li><em>models/engine/file_storage.py</em>: Class that serializes instances to a JSON file and deserializes JSON file to instances</li>
                    <li><em>models/__ init __.py</em>: A unique FileStorage instance for the application</li>
                    <li><em>models/base_model.py</em>: Class that defines all common attributes/methods for other classes.</li>
                    <li><em>models/user.py</em>: User class that inherits from BaseModel</li>
                    <li><em>models/state.py</em>: State class that inherits from BaseModel</li>
                    <li><em>models/city.py</em>: City class that inherits from BaseModel</li>
                    <li><em>models/amenity.py</em>: Amenity class that inherits from BaseModel</li>
                    <li><em>models/place.py</em>: Place class that inherits from BaseModel</li>
                    <li><em>models/review.py</em>: Review class that inherits from BaseModel</li>
   </ul>
   
   <H2>How to use it</H2>
   
   <p>This project is designed to work in two different modes, which includes:</p>
   <ul>
        <li><em>The Interactive mode</em></li>
        <li><em>The Non-interactive mode.</em></li>
  </ul>
   
   <p>The console in the interactive mode displays a prompt(hbnb) once a user writes or executes a command.<br>
     The prompt appears again after the command is run to wait for a new command.This is an indefinite process so long
     as the user does not terminate the program.</p>
    
      $./console.py
        (hbnb) help
            
        Documented commands (type help <topic>):
        ::::::::::::::::::::::::::::::::::
        EOF help quit<br>
            
        (hbnb)
        (hbnb)
        (hbnb) quit
      $
            
   <p>
        The shell in the <b>Non-interactive mode</b> needs to be run with a command input piped into its execution
        which enables the command to run once the shell starts operation. In this mode, no input is expected from the
        user
        therefore no prompt will appear.
    </p>
    
        $ echo "help" | ./console.py
        (hbnb)

        Documented commands (type help <topic>):
        ::::::::::::::::::::::::::::::::::::
        EOF help quit
        (hbnb)
        $
        $ cat test_help
        help
        $
        $ cat test_help | ./console.py
        (hbnb)

        Documented commands (type help <topic>):
        ::::::::::::::::::::::::::::::::::::::
        EOF help quit
        (hbnb)
        $


    
   <h2>Format of Command Input</h2>
   
   <p>This is necessary when giving command to the console. There ia the need for it to be piped through an echo 
      in case of the non-interactive mode.</p><br>
      <p>In Interactive Mode the commands will need to be written with a keyboard when the prompt appears and will
         be recognized when an enter key is pressed (new line). As soon as this happens, the console will attempt
         to execute the command through several means or will show an error message if the command didn't run
         successfully.<br>
         In this mode, the console can be exited using the CTRL + D combination, CTRL + C, or the command quit or
         EOF.</p>
         <h2>Arguments</h2>
