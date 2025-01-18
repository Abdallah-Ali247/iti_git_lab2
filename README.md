# Lab 2 Soloution Steps (Abdallah Ali Abdallah) 
  [Review Steps](Steps.txt)

## Removing Branches"
### Locally:
`git branch -d dev`
`git branch -d test`
### Remotely:
`git push origin --delete dev`
`git push origin --delete test` 

---

## Annotated Tags vs Lightweight Tags  

### Annotated Tags  
- Annotated tags store additional metadata such as the author's name, email, date, and a message.  
- They are stored as `full Git objects` and are useful for version releases.  

### Lightweight Tags  
- Lightweight tags are simple references to a specific commit, without additional metadata.  
- Useful for `temporary` or less formal uses.  

### When to Use  
- Use **annotated tags** for official releases and when metadata is important.  
- Use **lightweight tags** for quick references or internal purposes.  

---

## When to Use Rebase  

- **Use Rebase**:  
  - When working on feature branches to clean up commit history before merging.  
  - To update your branch with the latest changes from the main branch without creating a merge commit.  

- **Avoid Rebase**:  
  - On shared branches, as it rewrites commit history.  
  - When commit history needs to remain intact for auditing purposes.  

---

## How to List Tags  

To list all tags in the repository:  
 `git tag`

To list tags with details (annotated tags):
`git show <tagname>` like : `git show v1.7`

## How to Delete a Tag
### Locally
To delete a tag locally:
`git tag -d <tagname>`  

### Remotely
To delete a tag from the remote repository:
`git push origin --delete <tagname>`

## Add an Image
![Git Logo](https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png)  


