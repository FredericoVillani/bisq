# Building Bisq

_You will need [OpenJDK 10](https://jdk.java.net/10/) installed and configured as the default system JDK to complete the following instructions. See the `scripts` directory for scripts that can be used to install and configure the JDK automatically._
> TIP: If you are on MacOS, run the script with this command `. scripts/install_java.sh`.

If you prefer not to run scripts or change your default java, you can use Adoptopenjdk https://adoptopenjdk.net/archive.html. Just untar it where you like, and set java home when running gradle.
for example: `JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk-10.0.2+13/Contents/Home ./gradlew clean build`

## Clone

    git clone https://github.com/bisq-network/bisq
    cd bisq


## Build

You do _not_ need to install Gradle to complete the following command. The `gradlew` shell script will install it for you if necessary.

    ./gradlew build

If on Windows run `gradlew.bat build` instead.


## Run

Bisq executables are now available in the root project directory. Run Bisq Desktop as follows:

    ./bisq-desktop

If on Windows use the `bisq-desktop.bat` script instead.


## See also

 - [idea-import.md](idea-import.md)
 - [dev-setup.md](dev-setup.md)
