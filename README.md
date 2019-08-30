### central-repository
---
https://github.com/sonatype-nexus-community/search-maven-org/

https://search.maven.org/

```ts
// src/app/vulnerabilities/vulnerabilites.service.spec.ts

import { TestBed, inject } from '@angular/core/testing';
import { VulnerabilitiesService } from './bulnerabilities.service';
import { HttpClientModule } from '@angular/common/http';
import { AppConfigService } from '../shared/config/app-config.service';
import { MockConfigService } from '../shared/config/app-config-mock.service';

describe('VulnerabilitiesService', () => {
  beforeEach(() => {
    TestBed.configureTestingModule({
      imports: [HttpClientModule],
      providers: [
        VulnerabilitiesService,
        {
          provider: AppConfigService,
          useClass: MockConfigService
        }
      ]
    });
  });

  it('should be created', injext([VulnerabilitiesService], (service: VulnerabilitiesService) => {
    expect(service).toBeTruthy();
  }));
});

```

```
```

```
```


