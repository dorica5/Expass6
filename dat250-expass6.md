### Expass 6 Report

For this week the goal was to learn more about messaging. An asynchronous for two different applications to communicate. For this lab we had to use RabbitMQ, an open-source message broker.

##### Technical Problems
During the lab, most of the experiments went relatively smoothly without any problems. The place where i encountered an issue was with Experiment 3 while implementing Work Queues. For this part, even though i followed what the tutorials said, the `Worker` classes were not printing out anything no matter how many of them i run at the same time.  I tried different solutions including checking the RabbitMQ UI at localhost to verify that the messages were being sent to the correct queue (`task_queue`), which they were. I tried googling to see the issue, and i couldn't find a solution that worked for me.  This was the case until the very end and after verifying the queue declaration in both `NewTask` and `Worker` i restarted IntelliJ and Docker, which seemed to resolve the issue. The issue could have been because of this, or it could have been because i wasn't finished with writing all the code needed until the very end.

##### Unresolved Issues
During the tutorial, there were parts where we could for example list the exchanges that we have. When i tried to do this on my machine, i got an error. It was something about `rabbitmqctl` and i felt that these parts were not very necessary and therefore didn't really spend time trying to fix the issue. The tutorial is very command line based mostly with Unix systems, while i mostly used the IDE on my Windows machine.

##### Link to code
[Code for experiments 1-4]()

##### Conclusion
All in all this was a very fun and educational assignment. The RabbitMQ software is something i hadn't encountered before, and it was interesting seeing how messages could be implemented in an application.