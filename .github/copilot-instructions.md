# MuseumCheckAlias - GitHub Pages Domain Alias Repository

MuseumCheckAlias is a minimal GitHub Pages repository that serves as a domain alias for the Chinese domain `xn--9kroa195ivupp99b.cn`. This repository contains static files and configuration for GitHub Pages hosting.

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Working Effectively

### Repository Structure
- Bootstrap and explore the repository:
  - `cd /path/to/MuseumCheckAlias`
  - `git status`
  - `find . -not -path "./.git*" -type f` -- lists all non-git files
  - Repository contains only 2 files: `CNAME` and `Test`

### File Descriptions
- **CNAME**: Contains the custom domain configuration `xn--9kroa195ivupp99b.cn` for GitHub Pages
- **Test**: Minimal test file containing just `..` (2 bytes)

### No Build Process Required
- **CRITICAL**: This repository has NO build process, dependencies, or compilation steps
- **CRITICAL**: Do NOT look for package.json, Makefile, or build scripts - they do not exist
- **CRITICAL**: Do NOT attempt to run npm install, make, or any build commands
- Changes take effect immediately when pushed to GitHub

### Making Changes
- Edit files directly:
  - `git status` -- check current state
  - Edit CNAME to change domain alias: `printf "newdomain.com" > CNAME`
  - Add static content files as needed
  - `git add .` -- stage changes
  - `git commit -m "Description of changes"` -- commit changes
  - `git push origin [branch-name]` -- push to GitHub

### GitHub Pages Configuration
- GitHub Pages is automatically enabled for this repository
- Domain alias is configured via the CNAME file
- Changes to CNAME require DNS configuration at the domain provider
- Pages are served from the root directory of the default branch

## Validation

### Testing Changes
- **CRITICAL**: No automated tests exist - this is normal for this repository type
- Validate CNAME format: `cat CNAME` -- should contain only the domain name
- Check file encoding: `file CNAME` -- should be ASCII text
- Verify git status: `git status` -- should show clean working tree after commit

### Manual Validation Steps
- After making changes, verify the repository state:
  - `find . -not -path "./.git*" -type f` -- list all files
  - `git log --oneline -5` -- check recent commits
  - `wc -c CNAME` -- CNAME should be 23 bytes for current domain
  - `xxd CNAME` -- verify CNAME contains expected domain in hex

### Domain Validation
- **CRITICAL**: Domain accessibility depends on external DNS configuration
- Test domain resolution: `nslookup xn--9kroa195ivupp99b.cn` -- may fail if DNS not configured
- GitHub Pages URL: `https://jackandking.github.io/MuseumCheckAlias/`
- **DO NOT** expect immediate domain access after CNAME changes

## Common Tasks

### Repository Root Structure
```
ls -la /path/to/MuseumCheckAlias
.
..
.git/
CNAME
Test
```

### Current File Contents
```
cat CNAME
xn--9kroa195ivupp99b.cn

cat Test
..
```

### Git Operations
```
git status
# On branch [current-branch]
# nothing to commit, working tree clean

git log --oneline -3
# Shows recent commits
```

## Important Notes

### What This Repository IS
- A GitHub Pages domain alias configuration
- Static file hosting via GitHub Pages
- Simple domain redirection setup

### What This Repository IS NOT
- A software development project
- A repository requiring builds, tests, or complex CI/CD
- A repository with dependencies or package management

### Time Expectations
- **File edits**: Immediate (seconds)
- **Git operations**: 1-5 seconds each
- **GitHub Pages deployment**: 1-10 minutes after push
- **Domain propagation**: 24-48 hours for DNS changes

### Critical Reminders
- **NEVER** look for build files or attempt to build anything
- **NEVER** expect complex development workflows
- **ALWAYS** verify file contents after editing with `cat filename`
- **ALWAYS** check git status before and after changes
- Changes are deployed automatically via GitHub Pages when pushed

## Troubleshooting

### Common Issues
- Domain not accessible: This is expected if DNS is not configured at domain provider
- CNAME file corruption: Verify with `xxd CNAME` and recreate if needed
- Git conflicts: Use `git status` and resolve manually

### Emergency Recovery
- Restore CNAME: `printf "xn--9kroa195ivupp99b.cn" > CNAME`
- Check current state: `git status && find . -not -path "./.git*" -type f`
- Reset to last commit: `git checkout HEAD -- filename`