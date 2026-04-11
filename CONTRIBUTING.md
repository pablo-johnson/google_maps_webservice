# Contributing to google_maps_webservice

## What you will need

- A Linux, macOS, or Windows machine.
- Git for source control. See the [Git installation guide][git].
- The Dart SDK. See the [Dart SDK installation guide][dart].
- The Flutter SDK for running Flutter-based checks. See the [Flutter installation guide][flutter].
- A GitHub account. See [GitHub][github].

## Setting up your development environment

- Fork [google_maps_webservice][repo] into your own GitHub account.
- If you do not already have an SSH key configured for GitHub, follow the [GitHub SSH key guide][git-ssh].
- Clone your fork:

```sh
git clone git@github.com:<your_name_here>/google_maps_webservice.git
```

- Change into the project directory:

```sh
cd google_maps_webservice
```

- Add the original repository as the upstream remote:

```sh
git remote add upstream git@github.com:lejard-h/google_maps_webservice.git
```

## Running the example project

- Change into the example directory and set your API key:

```sh
cd example
export API_KEY="YOUR_KEY"

dart directions.dart
dart geolocation.dart
dart places_autocomplete.dart
```

## Contribute

We appreciate contributions via GitHub pull requests.

- Make sure your local branch is based on the latest upstream master branch:

```sh
git fetch upstream
git checkout upstream/master -b <name_of_your_branch>
```

- Apply your changes.
- Verify your changes and fix any warnings or errors:

```sh
dart pub get
dart format .
dart analyze
dart test
dart run build_runner build --delete-conflicting-outputs
```

- Commit your changes:

```sh
git commit -am "<your informative commit message>"
```

- Push changes to your fork:

```sh
git push origin <name_of_your_branch>
```

## Send us your pull request

Open [the repository][repo] and click "Compare & pull request".

Please make sure all formatting, analysis, tests, and generated files are up to date before opening the PR.

[git]: https://git-scm.com/
[flutter]: https://flutter.dev/docs/get-started/install
[github]: https://github.com/
[git-ssh]: https://help.github.com/articles/generating-ssh-keys/
[dart]: https://dart.dev/get-dart
[repo]: https://github.com/lejard-h/google_maps_webservice
