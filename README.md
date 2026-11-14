# heroku-buildpack-libredwg

Builds [LibreDWG](https://www.gnu.org/software/libredwg/) 0.14 from the GNU source tarball (checksum pinned) into the slug at `vendor/libredwg`, puts `dwg2dxf` on the PATH, and caches the build between deploys.

```bash
heroku buildpacks:add -i 1 https://github.com/PassivSure/heroku-buildpack-libredwg -a <app>
```

The source of truth is `vendor/buildpacks/libredwg/` in ps-rails; change it there and copy it here.
