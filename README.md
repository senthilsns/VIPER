# VIPER
Viper Architecture

Platform : XCode 10.1

Language : Swift 4.2

View: Class that has all the code to show the app interface to the user and get their response. Upon receiving the response View alerts the Presenter.

Presenter: Nucleus of a module. It gets user response from the View and work accordingly. Only class to communicate with all other components. Calls the router for wire-framing, Interactor to fetch data (network calls or local data calls), view to update the UI.

Interactor: Have business logics of an app. Primarily make API calls to fetch data from a source. Responsible for making data calls but not necessarily from itself.

Router: Does the wire-framing. Listen from the presenter about which screen to present and executes it.

Entity: Contains plain model classes used by interactor.

