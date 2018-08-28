swagger: "2.0"
x-collection-name: Trello
x-complete: 1
info:
  title: Trello
  description: this-document-describes-the-rest-api-of-trello-as-published-by-trello-com---a-hrefhttpstrello-comdocsindex-html-target-blankofficial-documentationa--a-hrefhttpstrello-comdocsapi-target-blankthe-html-pages-that-were-scraped-in-order-to-generate-this-specification-a
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /search:
    get:
      summary: Get Search
      description: Get search.
      operationId: getSearch
      x-api-path-slug: search-get
      parameters:
      - in: query
        name: boards_limit
        description: a number from 1 to 1000
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: cards_limit
        description: a number from 1 to 1000
      - in: query
        name: cards_page
        description: a number from 0 to 100
      - in: query
        name: card_attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: card_board
        description: true or false
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: card_list
        description: true or false
      - in: query
        name: card_members
        description: true or false
      - in: query
        name: card_stickers
        description: true or false
      - in: query
        name: idBoards
        description: A comma-separated list of objectIds, 24-character hex strings
      - in: query
        name: idCards
        description: A comma-separated list of objectIds, 24-character hex strings
      - in: query
        name: idOrganizations
        description: A comma-separated list of objectIds, 24-character hex strings
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: members_limit
        description: a number from 1 to 1000
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: modelTypes
        description: 'all or a comma-separated list of: actions, boards, cards, members
          or organizations'
      - in: query
        name: organizations_limit
        description: a number from 1 to 1000
      - in: query
        name: organization_fields
        description: 'all or a comma-separated list of: billableMemberCount, desc,
          descData, displayName, idBoards, invitations, invited, logoHash, memberships,
          name, powerUps, prefs, premiumFeatures, products, url or website'
      - in: query
        name: partial
        description: true or false
      - in: query
        name: query
        description: a string with a length from 1 to 16384
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Search
  /search/members:
    get:
      summary: Get Search Members
      description: Get search members.
      operationId: getSearchMembers
      x-api-path-slug: searchmembers-get
      parameters:
      - in: query
        name: idBoard
        description: An id, or null
      - in: query
        name: idOrganization
        description: An id, or null
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 20
      - in: query
        name: onlyOrgMembers
        description: A boolean
      - in: query
        name: query
        description: a string with a length from 1 to 16384
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Search
      - Members