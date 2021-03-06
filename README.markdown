Play Push
==========

## Introduction

This is a demo application that realizes a simple chat system using the Cappuccino Framework (http://www.cappuccino.org) as the client and the Play! Framework. (http://www.playframework.org) as the server. The client will request new messages from the server using an AJAX connection, while the server will suspend that 
connection for a second each time it can't deliver new messages. This will keep the connection open as long as there are no new messages. Upon receipt of new messages, 
the connection will close and the client will reopen another connection to wait for even more messages, and so on. 

This application is based on Elias Klughammer's explorations of Cappuccino, Tornado and Juggernaut, which he published here: http://github.com/eliasklughammer/Cappuccino-X-Tornado and here: http://github.com/eliasklughammer/Cappuccino-X-Juggernaut 

He also published a video demoing his app, which should be pretty similar to Play Push: http://www.youtube.com/watch?v=1MPTxS9uyT4

Thanks a lot for sharing, Elias! 

## Installation

__1. Download and install Play!__

Follow the instructions at http://www.playframework.org/documentation/1.0/install -- but *use a nightly build of the 1.1 branch* with a version of at least 722 or check out the trunk of the 1.1 branch and build Play! from source. Download the nightly build here: http://download.playframework.org/1.1-nightly/ Once Play! 1.1 is out, you may of course use the official release. 

__2. Clone this repository__

Clone or download this repository, you probably know how (hint: there is a link titled "Download Source" in the upper right of the page). 

__3. Start the Play! application__

Go to this repository's root folder and issue ´play run´ at the command line. 

__4. Go to http://localhost:9000 in your Browser__

Enter a username and enter some messages. Use additional browser windows to chat with yourself. 
