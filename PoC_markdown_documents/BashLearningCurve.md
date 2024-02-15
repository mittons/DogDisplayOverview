# BashLearningCruve

Lists a few of my bash files (or specific commit changes to them) in the past month or two, in order show showcase my growth and aquired learning with bash.


## My learning curve over time (with references to code and timestamps)

Jan 19, 2024 - [Build script from DogDisplayForC++ project](https://github.com/mittons/DogDisplayForCpp/blob/ac6c71918f26355d47a14db85fbb8d74e8c6c469/build_script.sh)
 - Basic sequence, small.

Jan 29, 2024 - [Build script from DogDisplayForPHP project](https://github.com/mittons/DogDisplayForPhp/blob/master/setup_php/php_setup_script.sh#L50)
  - Much longer than the previous expample, using loops now.
  - The link highlights my bash skills as of Jan 29, 2024, starting from line 51, showcasing [throughly-tested, solid code.](## "Through a hellish experience, debugging my initial approach, figuring out how to build PHP from source over 2 days of hardcore coding.")
  - <ins>Notice</ins>: *This example is* ***actually*** [*broken code (the first 50 are lines wrong!)*](## "In fact the first 50 lines, are not bash script, but the github actions script.. honest im not sure which way I translated it. I definitely made this script in bash first (it was a special hell over 2 days learning to build php from source in a fresh ubunut environment), but the bash code in this file might actually be translation of a GH actions script, that was translated from the original bash code. Anyway. 50 lines of bad code. Bad."), shame on me! Shame! Shame! 🔔. Shame! 🔔🔔.
  - I figure this code example could also be strong argument for peer review, and code review in general. *(Although, tecnically this "code file" is closer to documenation than code).*

Feb 11, 2024 - [Build script from DogDisplayStaticClient project](https://github.com/mittons/DogDisplayStaticClient/blob/main/deployment_scripts/build_e2e_tests.sh)
 - Move complex, using input args, usage instructions and more complex loops

Feb 11, 2024 - [Process running script from DogDisplayStaticClient project](https://github.com/mittons/DogDisplayStaticClient/blob/main/dev_scripts/run_test_helper_services.sh)
 - Spawning child processes, using signals an traps for cleanup.
