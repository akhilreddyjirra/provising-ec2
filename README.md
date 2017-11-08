List of all tasks in playbook
* `ansible-playbook playbook.yml --list-tasks`

Start the play from a particular task
* `ansible-playbook playbook.yml --start-at-task="task name"`

Start the play step by step with interactiveway.This will promt the user for to conform each task before running.
* `ansible-playbook  playbook.yml --step`

Check the syntax of the playbook
* `ansible-playbook palybook.yml --syntax-check`

Ececute the palybook in the check(dry-run)mode,which check what changes will be proformed
 * `ansible-playbook playbook.yml --check`

List hosts on which playbook will be executed
 * `ansible-playbook playbook.yml --list-hosts -l subset`

list tags in the playbook
 * `ansible-playbook playbook.yml --list--tags`

Only run play and tasks tagged with these tag valuses
 * `ansible-playbook playbook.yml --tags tag1,tag2...,tagN`

Skip the task associated with specific tasks
* `ansible-playbook playbook.yml --skip-tags tag1,tag2,....tagN`

The --fork what lets ansible run on multiple hosts in parrel NUM is specified as intiger the default is 5
 * `ansible-playbook playbook.yml --forks=NUM`

Run playbook on the target hosts with out inventory files
* `ansible-playbook playbook.yml -i (IP | SERVERNAME)`,
