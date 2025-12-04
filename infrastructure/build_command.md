| **命令**            |  **示例**                               | **描述**                                                     | **谁能使用**                                                 |
| ------------------- |  -------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| /[remove-]kind      | /kind bug   <br>/remove-kind bug           | 添加或者删除这种kind类型的标签。 例如：`kind/bug`标签。      | 任何人都能在一个Pull Request或者Issue上触发这种命令。        |
| /lgtm [cancel]      | /lgtm   <br>/lgtm cancel      | 为一个Pull Request添加或者删除`lgtm`标签，这个标签将用于Pull Request合入判断。    | 这个仓库的协作者。Pull Request能使用`/lgtm cancel`命令，但是不能使用`/lgtm`命令。   |
| /approve [cancel]     | /approve<br>/approve cancel          | 为一个Pull Request添加或者删除`approved`标签，这个标签将用于Pull Request合入判断。 | 这个仓库的协作者。   |
| /[remove-]priority  | /priority high <br> /remove-priority high | 添加或者删除这种priority类型的标签。 例如：`priority/high`标签。 | 任何人都能在一个Pull Request或者Issue上触发这种命令。        |
| /[remove-]team       | /team spec  <br> /remove-team spec | 添加或者删除这种team类型的标签。 例如：`team/spec`标签。  | 任何人都能在一个Pull Request或者Issue上触发这种命令。        |
| /close | /close | 关闭一个Pull Request或者Issue。 | 作者和仓库的协作者能触发这种命令。|
| /reopen | /reopen | 重新打开一个Issue。 | 作者和仓库的协作者能触发这种命令。|
| /assign [[@]...]    |  /assign @cangjiepl       | 分配一个Issue给负责人。                                      | 任何人都能在一个Issue上触发这种命令， 但是目标负责人必须是这个组织的一个成员。  如果没有指定目标负责人，这表明这个Issue会分配给自己。 |
| /unassign [[@]...]  | /unassign @cangjiepl   | 取消分配一个Issue给负责人。                                  | 任何人都能在一个Issue上触发这种命令， 但是目标负责人必须是这个组织的一个成员。  如果没有指定目标负责人，这表明这个Issue会取消分配给自己。 |
| /check-issue        | /check-issue                           | 检查Pull Request是否关联了Issue，如果未关联Issue，添加needs-issue标签，如果已关联，则删除`needs-issue`标签。 | 任何人都能在一个Pull Request上触发这种命令。                 |
| /remove-needs-issue | /remove-needs-issue                    | 删除`needs-issue`标签。                                        | 只有仓库成员才能在Pull Request上触发这种命令。               |