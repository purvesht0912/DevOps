# DevOps

some data
Configure a CI/CD pipeline file tro include a shedulded job that run minute using Gitlabs sheduling job that runs every minute using Gitlabs sheduling figure. verify the pipeline  execution by checking the jobs logs(i dont know anything , this qutin ask in preivious yeAR qutin paper answer i want write in short paper sheet , give answer towrite in paper sheet , also make sure its help in showing practicle to examiner , this qutions in DevOps lab practicle exam )

Use dockerr to modify and exeisting image , commit and save it as a new one.

Here’s a short and clear answer you can write on your paper sheet for your **DevOps lab practical exam**, based on the question:

---

**Q: Configure a CI/CD pipeline file to include a scheduled job that runs every minute using GitLab’s scheduling. Verify execution by checking job logs.**

**Answer (to write in paper):**

1. **Create `.gitlab-ci.yml` file:**

```yaml
stages:
  - scheduled

run_every_minute:
  stage: scheduled
  script:
    - echo "This job runs every minute"
```

2. **Setup Scheduled Job in GitLab UI:**

* Go to: `Project → CI/CD → Schedules → New schedule`
* Set **Interval pattern** to: `* * * * *` (every minute)
* Set **Target branch**: `main` (or your working branch)
* Click **Save**

3. **Verify Job Execution:**

* Go to: `CI/CD → Jobs`
* Check status and logs of `run_every_minute` job
* Click on the job to **view logs/output**

---

**Practically show this to examiner:**

* Open GitLab project
* Show `.gitlab-ci.yml`
* Open **Schedules** and show config
* Go to **CI/CD → Jobs**
* Click on recent job → show log output

---

Let me know if you want a handwritten-style version or translation in Hindi too.


Here is a **short and clear answer** you can write on a paper sheet for your **DevOps lab practical exam**, based on the question:

---

**Q: Use Docker to modify an existing image, commit and save it as a new one.**

**Answer (to write in paper):**

1. **Run a container from an image (e.g. ubuntu):**

```bash
docker run -it ubuntu
```

2. **Make changes inside the container** (example):

```bash
apt update && apt install -y curl
exit
```

3. **Find container ID (or name):**

```bash
docker ps -a
```

4. **Commit changes to a new image:**

```bash
docker commit <container_id> my_ubuntu_with_curl
```

5. **Verify new image is saved:**

```bash
docker images
```

---

**Practically show this to examiner:**

* Show `docker run`
* Do some change (install package)
* Exit and commit
* Show `docker images` with new image

---

Let me know if you want it translated into Hindi or handwritten style.




